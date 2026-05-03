# Mission Planning Essentials: Charts, JSA and NOTAMs

Before you fly, you need to know how to find the right aviation documents, prepare a proper Job Safety Assessment, and submit NOTAMs when required. These are the practical tasks that trip up new ReOC holders — not because they're difficult, but because nobody walks you through where things actually are.

This guide covers accessing aviation charts and aerodrome data, preparing a JSA that will hold up under audit, and setting up your NAIPS account for NOTAM briefings and submissions.

Author: Rachel Ng

Last review: 3 May 2026

---

## 1. Accessing Charts and Documentation

All the aviation documents you need for mission planning are available free through Airservices Australia.

1. Go to the [Airservices Australia AIP page](https://www.airservicesaustralia.com/aip/aip.asp)
2. Scroll to the bottom and click "Agree" to accept the terms
3. You'll see a list of available resources, select the most recent version (the date beside each item is the effective-from date)

### Charts You Need to Know

**VTC (Visual Terminal Chart)** — Your go-to for flying around controlled airports. Shows the most detail including CTR/CTA boundaries, restricted and danger areas, and local features. Start here when planning any operation near a controlled aerodrome.

**VNC (Visual Navigation Chart)** — Covers larger areas at lower detail than VTC. Use this for en-route navigation and lower-level operations. If your area isn't on a VTC, check the VNC.

**PCA (Planning Chart Australia)** — Big-picture overview of Australian airspace. Useful for initial planning but not detailed enough for operational decisions.

**Priority order:** Always check VTC first (most detail), then VNC, then PCA if still not found.

To access the charts, navigate to the charts section on the AIP page, select your region, and the chart opens as a PDF.

### ERSA (En Route Supplement Australia)

ERSA contains detailed aerodrome data — procedures, radio frequencies, runway info, and special conditions. This is where you confirm the specifics of any aerodrome near your operation.

To look up an aerodrome, scroll through the ERSA list, find the aerodrome relevant to you, and click "FAC" to open the PDF with that aerodrome's information.

For restricted areas (SUA — danger, prohibited and restricted areas), identify the restricted area code on your VTC/VNC chart first, then look it up in ERSA for the full details including activation times and conditions.

### DAH (Designated Airspace Handbook)

The DAH covers airspace classifications, restrictions, helicopter landing sites (HLS) and aircraft landing areas (ALA).

Key sections for RPAS operators:

- **Section 20** — HLS and ALA listings
- **Intro-2** — Latitude/longitude format standard (CASA expects aviation-standard formatting in your mission planning documents)

### How This Applies to Your ReOC Operations

These aren't just reference documents — CASA expects you to demonstrate you can use them.

- **ERSA:** Look up nearest aerodrome procedures, traffic frequencies, and special procedures. This demonstrates you can operate safely near manned aviation.
- **VTC/VNC:** Use in planning to identify controlled airspace, CTR/CTA boundaries, restricted and danger areas. CASA may ask you to show on a chart how you confirmed whether your mission is inside controlled airspace.
- **DAH:** Check restricted and prohibited airspace, plus HLS/ALA near your operation area.
- **Lat/Long format:** Use the aviation-standard format from DAH Intro-2 when documenting site coordinates in your planning documents and Form 101-09 submissions.

> **Tip:** Save or print the VTC/VNC charts for your regular operational areas. Practice looking up an aerodrome in ERSA. If you're going through a CASA assessment, be ready to demonstrate *how* you found the information, not just give the answer.

---

## 2. Preparing a Job Safety Assessment (JSA)

A JSA breaks your operation into steps, identifies hazards at each step, and documents the controls you'll put in place. CASA expects a site-specific JSA for each operation — not a generic template with boxes ticked.

### What Your Drone JSA Should Cover

**Job details at the top:**

- Date, location, client name
- Pilot name(s) and CRP sign-off
- Aircraft type and registration
- CASA approval reference (if applicable)

**Site-specific information:**

- Map or screenshot of the operational area showing takeoff/landing sites, observer positions, exclusion zones, safe zones, and signage locations
- Nearest aerodrome and distance
- Airspace classification
- Radio frequencies (CTAF or ATC as applicable)

**Task steps with hazards and controls:**

Break the operation into sequential steps (setup, pre-flight checks, flight, landing, pack-down) and for each step identify what could go wrong and what you'll do about it.

### Common Drone Operation Hazards to Address

| Hazard Category | Examples | Typical Controls |
|---|---|---|
| **Airspace** | Manned aircraft in vicinity, proximity to aerodrome | Monitor CTAF/ATC frequency, maintain VLOS, land if manned traffic detected |
| **Weather** | Wind exceeding limits, sudden changes, rain | Check BOM and NAIPS forecasts, set wind limits per aircraft specs, abort criteria |
| **Ground hazards** | Powerlines, trees, buildings, people | Site survey, exclusion zones, observers, minimum standoff distances |
| **Public/bystanders** | Unauthorised people entering area | Signage, barriers, observers, brief crew on crowd management |
| **Equipment failure** | Battery failure, signal loss, GPS dropout | Pre-flight checks, RTH settings, failsafe configuration, spare batteries |
| **Emergency** | Flyaway, crash, injury | Emergency procedures documented, first aid kit on site, emergency contacts listed |

### What Makes a Good JSA vs a Bad One

**Good JSA:** Site-specific hazards identified from an actual site survey or desktop reconnaissance. Controls are practical and measurable ("maintain 30m lateral separation from powerlines" not "be careful near powerlines"). Risk ratings reflect the actual scenario after controls are applied.

**Bad JSA:** Generic hazards copied from a template with no reference to the actual site. Controls are vague. Same JSA used for every job with only the date changed. This is the "tick-and-flick" approach — CASA auditors will spot it immediately.

### Risk Assessment

Your JSA should include or reference a Risk Assessment (RA) using a risk matrix. For each hazard, assess the likelihood and consequence both before and after controls are applied. Your Operations Manual should define the risk matrix your organisation uses.

The RA must be specific to the mission. If you're submitting with a Form 101-09 application, CASA reviewers will check that the RA addresses the specific risks of the site and operation type — not just generic drone risks.

---

## 3. NAIPS: Account Setup and Using NOTAMs

NAIPS (National Aeronautical Information Processing System) is the platform run by Airservices Australia that provides real-time aeronautical data, weather information, and NOTAMs. As a ReOC holder, you need a NAIPS account for pre-flight briefings and NOTAM submissions.

### Creating Your NAIPS Account

1. Go to the [NAIPS registration page](https://www.airservicesaustralia.com/naips/Account/Register)
2. Register a username and password and provide your contact details
3. Your login credentials also give you access to the NAIPS Internet Service (NIS) for briefings and NOTAM checking
4. Keep your credentials secure — you're responsible for any activity under your account

Registration is free. Once registered, you can log in at the [NAIPS Internet Service](https://www.airservicesaustralia.com/naips/Account/Logon).

> If you need help with the NAIPS system, contact the Airservices Service Desk (24/7) on **1800 801 960**.

### What You Use NAIPS For

**Pre-flight briefings:** Before every operation, check NAIPS for current NOTAMs affecting your area. Use a Location Briefing for information around a specific aerodrome (covers 5 NM radius), or an Area Briefing for a broader region.

**Weather data:** Access TAFs (Terminal Area Forecasts), METARs, and other meteorological information for your area.

**NOTAM checking:** Verify that your own NOTAM is active on the day of operations, and check for other NOTAMs that might affect your flight (temporary restricted areas, military exercises, emergency operations, etc).

> **Important:** Not all aerodromes have a NOTAM service. If you request a briefing for an aerodrome without one, NAIPS will tell you "A NOTAM service is not provided for the following location" — this doesn't mean there are no NOTAMs, it means that aerodrome isn't covered.

### Submitting NOTAMs for Your Drone Operations

If your CASA approval conditions require a NOTAM (many area approvals do), you'll need to submit one before each operation. CASA will specify the NOTAM requirements in their approval instrument — read it carefully.

**Timing:** Submit your NOTAM to CASA at least **2 business days** before the flight. CASA will coordinate with Airservices for promulgation. Allow time for any back-and-forth.

**How to submit:** CASA will provide guidance on the NOTAM submission process in their approval email. Typically this involves completing the Airservices NOTAM Request Form and submitting it as directed. Airservices has also rolled out a NOTAM Web Service (NWS) within NAIPS, which allows authorised originators to enter NOTAM information directly via a web form instead of emailing PDF forms.

**On the day:** Before you fly, log into NAIPS and confirm your NOTAM is active and correct. Also check for any other NOTAMs in your area that may have been published since you last checked.

### NAIPS Mobile Access

The NAIPS app (available on iOS, developed by OzRunways) lets you access briefings, submit flight notifications, and check NOTAMs from your phone. Useful for on-site checks, but you still need your NAIPS login credentials.

Other CASA-verified apps like OzRunways and AvPlan also integrate NOTAM data from Airservices Australia.

---

## Putting It All Together: Pre-Mission Workflow

Here's how these pieces fit into your planning sequence:

1. **Confirm the job** — Get operational details and location from the client
2. **Check airspace** — Use VTC/VNC charts and ERSA to identify airspace classification, nearby aerodromes, restricted areas, and radio frequencies
3. **Determine if CASA approval is needed** — See our [CASA Approvals guide](casa-approvals-application.md)
4. **Conduct site reconnaissance** — Desktop or physical site survey to identify hazards
5. **Prepare your JSA and Risk Assessment** — Site-specific, referencing your actual findings from steps 2 and 4
6. **Prepare your Flight Plan** — Including site coordinates in aviation format (DAH Intro-2)
7. **CRP review and sign-off** — Per your Operations Manual procedures
8. **Submit NOTAM** — If required by your approval conditions, at least 2 business days before
9. **Pre-flight NAIPS check** — On the day, confirm your NOTAM is active, check weather, and review any new NOTAMs in your area
10. **Fly the mission** — Comply with your approval conditions, JSA controls, and standard drone rules

---

## Useful Links

- [Airservices Australia — AIP, Charts and ERSA](https://www.airservicesaustralia.com/aip/aip.asp)
- [NAIPS Registration](https://www.airservicesaustralia.com/naips/Account/Register)
- [NAIPS Login](https://www.airservicesaustralia.com/naips/Account/Logon)
- [NAIPS Internet Service User Guide (PDF)](https://www.airservicesaustralia.com/naips/Content/Files/documents/NAIPS-Internet-Service-User-Documentation.pdf)
- [Airservices NOTAM Originator Resources](https://www.airservicesaustralia.com/industry-info/flight-briefing/notam-originator/)
- [CASA Verified Drone Safety Apps](https://www.casa.gov.au/knowyourdrone/drone-safety-apps)
- [CASA Standard Drone Rules](https://www.casa.gov.au/knowyourdrone/drone-rules)
- Airservices Service Desk (24/7): **1800 801 960**

---

> **Disclaimer:** This article is for general educational purposes only and does not constitute legal or regulatory advice. Always refer to the [CASA website](https://www.casa.gov.au), [Airservices Australia](https://www.airservicesaustralia.com), and current legislation for the latest requirements. Procedures, forms and systems may change without notice.

*This article is part of the [OpenReOC](https://github.com/rachelng-rpas/openreoc) series — practical guides for Australian drone operators navigating CASA regulations.*
