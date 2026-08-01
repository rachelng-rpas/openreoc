# Building "Sortie": An AI-Assisted Development Log

A record of how a working operational tool was built through iterative prompting with Claude (Anthropic), kept here as a learning log rather than a product spec. Company, client, and site-specific details have been generalised or removed — this is about the *process*, not the deployment.

---

## 1. The problem I was trying to solve

I work in a Remote Operations Centre (ROC) coordinating BVLOS (beyond-visual-line-of-sight) drone survey flights from a fixed dock. Each fortnight, a client supplies dozens to hundreds of individually pre-planned flight routes (as KMZ files), and my job includes:

- Figuring out which routes are close enough together to fly on a single battery charge
- Proposing a bounded "operation area" to the client for the next fortnight, which needs resident/stakeholder sign-off before flying
- Producing a client-facing document, a pilot-facing summary, and a Slack update — every cycle, by hand

Before this project, all of that was done by eye on a map covered in scattered route lines, plus manual retyping of the same kind of summary message each time. I wanted to see how far I could get automating the geometry and the repetitive parts while keeping every real judgement call in my own hands.

## 2. Tools and approach

Built entirely through conversation with Claude, using its ability to write and iterate on a single self-contained HTML/JS file (no backend, opens directly in a browser). No manual coding on my part — every change was described in plain language, usually anchored to a screenshot of what was and wasn't working.

The rough shape of the workflow, cycle after cycle:

1. Describe a problem or paste a screenshot of the current behaviour
2. Claude proposes an approach (sometimes asking me to choose between options before building, for anything with real operational judgement in it — e.g. "what rule should decide if two routes share a battery?")
3. It builds/edits the file and hands back a new version
4. I test it against real data, screenshot whatever's broken or awkward, and we go again

A pattern that turned out to matter a lot: for anything touching real flight-safety judgement (distance budgets, no-fly thresholds, how areas get approved) I asked Claude to explain the trade-offs and propose options rather than just implement its first idea — and for anything more mechanical (styling, a button label, a bug fix) I just described the symptom and let it fix it directly. That split kept iteration fast without rubber-stamping decisions that actually mattered.

## 3. Development timeline

### Phase 0 — Requirements before code
Before any building started, I described the manual process (screenshots of the existing map-based workflow, an explanation of the Google Drive folder structure routes were stored in, the physical constraints of the drone/battery) and asked for an analysis of what the tool should do *before* writing anything. This produced a proposed feature list and a short round of clarifying questions (how files would be imported, how grouping should work, what output formats were needed) before the first line of code was written.

### Early build — first working version
- Core scaffold: interactive map, KMZ import, a route list, manual and automatic grouping into "batteries," KMZ export.
- **First real bug, and a good example of why testing against real data matters**: the KMZ parser assumed the standard KML convention (one route = one connected line). The actual files — exported from DJI's flight-planning software — use a different internal format where a whole mission is stored as dozens of separate single-point placemarks in an unnamed folder, not a line. Every waypoint was being imported as its own route. Fixed by having Claude inspect the actual file structure (unzipping and reading the raw KML) rather than assuming the format, then writing a parser that handles the real shape.
- Import de-duplication, status-tagged imports (pending vs. completed), and safer duplicate-handling followed from real usage friction ("I re-imported the same folder and got duplicates").

### Mid build — no-fly logic, area generation, records
- Added a proper no-fly classification system: a hard exclusion zone (polygon-based) plus a softer distance-based threshold, both configurable rather than hardcoded, after discussing the actual battery-consumption math with me (this became a running theme — several of the tool's constants trace back to a short back-and-forth about real drone/battery behaviour rather than an arbitrary default).
- The area-proposal tool went through a genuine design iteration: the first version drew a convex hull around all pending routes, which produced oddly-shaped, multi-directional blobs whenever routes were scattered in different compass directions. Reworked into a proper single-direction "pie slice" construction (bearing from the hub, angular sector, capped radius) after I flagged the visual problem with a screenshot.
- Later replaced with a manual click-to-draw tool as the primary method (the algorithm demoted to an optional starting point), because a mathematically tidy shape doesn't always match what should actually be proposed to a client.
- Added a records/audit view (completed, incomplete, "attempted but couldn't be flown" with a note field) after realising a route that failed mid-flight needed to be remembered, not silently re-scheduled.

### Later build — map clarity, real satellite exports, and a genuine debugging dead-end
- Switched the basemap and colour palette after feedback that the map was hard to read; compared against a reference tool I liked the look of.
- **The most interesting technical dead-end of the project**: the client-facing PDF and pilot-facing image were originally built by screenshotting the live interactive map. This worked in simple cases but silently dropped most of the overlay content (routes, boundaries) in real use — turned out to be a known, non-obvious interaction between the mapping library's use of CSS transforms for smooth panning/zooming and the screenshot library's inability to capture transformed content correctly. Rather than patch around it, the fix was to stop screenshotting entirely: fetch the same satellite tiles directly and draw the overlays by hand using the same map-projection maths the tiles use, guaranteeing the export always matches what was drawn — no dependency on a screenshot library's quirks. A good lesson in recognising when a symptom points to a fundamental tool mismatch rather than a timing bug.
- Removed a "requires manual confirmation" step once I pointed out it was pure duplicated effort — drawing the operation area already *was* the confirmation of which routes were included; a separate tick-box step was just friction.
- Tried, tested, and then deliberately reverted a "shared, multi-user" data mode after clarifying the actual usage pattern was one operator distributing exported outputs manually, not multiple people editing live together.

### Recent build — packaging for real operational use
- Bulk import matched to the actual Drive folder structure the client data already lived in (three subfolders, each implying a different route status), so a whole fortnight's backlog imports in one action instead of one file at a time.
- Split "background settings" (thresholds, no-fly data, approved boundary) into a separate settings view from the weekly workflow, once the main screen started feeling cluttered with things that only get touched occasionally.
- Added the pilot-facing colour-coded image export and an automatic Slack-message generator that fills in a fixed message template with live numbers (route counts, batch breakdown, distances/times) — built from a real example message I supplied, so the tone and structure matched what the team already expected to see.

## 4. What I'd call out as genuine learning moments

- **Don't trust a file format until you've actually opened one.** The DJI KMZ bug only got found by unzipping a real file and reading it, not by assuming a spec.
- **A tool failing "successfully" is worse than an error.** The screenshot-capture bug didn't crash — it just quietly produced a plausible-looking but wrong image. Worth specifically testing rendered output, not just "did it run."
- **Ask for the option set before the code, on anything with real judgement in it.** The battery-grouping algorithm and the no-fly thresholds both went through a "here are the trade-offs, which do you want" conversation before implementation — cheaper to have that conversation in plain language than to build the wrong thing and redo it.
- **Removing a feature is sometimes the fix.** More than one round of "fixing" this tool was actually deleting a step (a redundant confirmation click, a duplicate export button, a second competing "area" concept) rather than adding anything.
- **Iterating against real screenshots beats describing bugs in prose.** Almost every meaningful bug fix in this project started with a screenshot of the actual broken state, not a text description of the symptom.

## 5. What the tool does today (summary)

- Imports flight-route KMZ files in bulk, auto-detecting status from folder structure
- Flags routes that are too far to attempt or fall inside a no-fly area
- Auto-groups remaining routes into battery-sized batches by proximity and a configurable distance budget
- Lets the operator draw (or auto-suggest) the fortnight's proposed operation area directly on the map
- Generates a client-facing PDF, a matching KMZ for GIS tools, a pilot-facing summary image, and a ready-to-post team update — all from the same confirmed data, no retyping

---

*This log covers the process, not the deployed configuration — thresholds, coordinates, and client/site identifiers used in the live tool are specific to one operational context and have been left out here.*
