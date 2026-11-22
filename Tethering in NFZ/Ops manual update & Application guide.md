# Tethering in No-Fly Zone (NFZ) — ReOC Upgrade Guide & Template

> Guidance document from the OpenReOC project. Developed from operational
> experience reviewing a ReOC Operations Manual upgrade (v1 → v2 → v3) and a
> real CASA significant-change submission, **approved on 17 Nov 2026**.
> Last updated: 22 Nov 2026.
>
> This is **not** a regulatory document — always check the current Part 101 MOS,
> CASR, and applicable CASA instruments before relying on any clause numbers below,
> as these change periodically.
>
> Companion files in this folder: [Case study and Fee](Case%20study%20and%20Fee.md) ·
> [MOS clause quick reference](MOS%20clause%20quick%20reference.md) ·
> [Scenario questionnaire — how to prepare](Scenario%20questionnaire%20-%20how%20to%20prepare.md)

---

## 1. Why tethering in a no-fly zone (NFZ) needs separate approval

A standard ReOC, even one that already permits tethered operations, does **not**
automatically allow tethering inside the no-fly zone of a controlled or
non-controlled aerodrome (the "black" and "grey" shaded areas around an
aerodrome, including the 3 NM zone).

### What the base ReOC typically says (and doesn't say)
In the initial Operations Manual, the "Tethered operations" policy section
already states, in effect:

- The CRP may approve tethered operations.
- CASA approval is required for tethered operations in the no-fly zone of a
  **controlled aerodrome**.
- Tethered operations within the no-fly zone of a **non-controlled aerodrome**
  are allowed without extra CASA approval, provided the relevant standard is
  met, and are permitted during relevant events.
- For specialised tethered procedures, refer to Appendix D.

So the base manual already **flags** that controlled-aerodrome NFZ tethering
needs separate CASA approval — but it does not grant that approval, and the
corresponding appendix section ("Tethered operations within the no-fly zone of
a controlled aerodrome") is left as **"Reserved"** — i.e. there is no actual
procedure written to support it.

### What this means in practice
- The base ReOC's tethered operations policy **only operationalises** tethering
  **outside** the no-fly zone of a controlled aerodrome (under standard tether
  limitations), and tethering inside the NFZ of a non-controlled aerodrome
  (which doesn't need extra approval).
- Tethering inside the no-fly zone of a **controlled aerodrome** is explicitly
  carved out by the manual's own wording as requiring CASA approval — and
  because the supporting appendix is "Reserved", there is no documented
  procedure for the CRP to approve against, and no basis to apply to CASA for
  approval yet.
- Tethered operations within **restricted/military controlled airspace** sit
  outside this entirely and require a valid Letter of Agreement (LOA) from the
  controlling authority, with clearance obtained before each take-off.

### The bottom line
The base ReOC already tells you that controlled-aerodrome NFZ tethering needs
CASA approval — it just doesn't contain the procedure or the approval itself.
To actually fly tethered inside a controlled aerodrome's no-fly zone, the
operator must write the missing Appendix D procedure, get it approved by CASA
as a significant change to the ReOC, and only then can the CRP approve
individual flights against it.

### Legal basis and what CASA actually approves

The permission to fly tethered inside a controlled aerodrome's no-fly zone comes
from the Part 101 MOS, not from the ReOC itself (clause detail in the
[MOS clause quick reference](MOS%20clause%20quick%20reference.md)):

- **MOS 4.03(1)** prohibits RPA operations and flights in the no-fly zone of a
  controlled aerodrome, subject to exceptions.
- **MOS 4.03(2)** lets a *certified RPA operator* (or its remote pilot) conduct a
  **tethered operation** in that zone if it complies with **MOS 4.04**.
- **MOS 4.04(3)** sets the conditions: tether no longer than 150 ft; RPA no higher
  than 150 ft above aerodrome elevation; flown per the operator's *documented
  practices and procedures*; ATC notified before take-off and ATC instructions
  followed; and either in the grey area or — if in the black area — not within
  3 NM of a runway measurement point.

Because 4.04(3)(c) ties the operation to your documented practices and
procedures, what CASA approves is **the procedures in your Operations Manual**, as
a *significant change* under **MOS 10A.01**. In the case documented here the
approval letter:

- named the Operations Manual version and date that was approved,
- confirmed the change was consistent with the nature and scope of the ReOC and
  would have no adverse effect on aviation safety, and
- stated the ReOC did **not** need to be reissued.

The inspector also confirmed that, for a significant-change-only application,
*acceptance of the manual constitutes the approval*.

> **Worth reviewing in your own manual:** the template wording in section 5.4 says
> tethered NFZ operations "must not be conducted without prior CASA approval". Read
> against MOS 4.03(2) and 4.04(3), the MOS conditions are met by following your
> approved procedures — CASA approves the procedures, not each flight. In the case
> documented here the manual contained similar "CASA approval required" wording and
> CASA did not query it, but check that your manual doesn't promise a per-flight
> CASA approval you don't intend to seek.

**A different route — area approval.** Operating near a controlled aerodrome can
also be authorised through an area approval (Form 101-09, CASR 101.030 — see
[Form 101-09 Area Approval](../CASA%20approvals%20application/Form%20101-09%20Area%20Approval.md)).
The tethering route in this guide doesn't use that form: it relies on MOS 4.03(2)
and 4.04, with your procedures approved through the significant-change process.

---

## 2. What needs to change to be allowed to fly tethering in NFZ

To extend an existing ReOC to cover tethered operations in the no-fly zone of a
controlled aerodrome, the operator generally needs to:

1. **Add a dedicated procedure/section** to the Operations Manual specifically
   covering "Tethered operations within the no-fly zone of a controlled
   aerodrome" — separate from, and in addition to, the general tethered
   operations procedure.
2. **Rephrase the general tethering policy section** to clearly distinguish:
   - tethering outside NFZ (covered by existing ReOC),
   - tethering inside NFZ of a controlled aerodrome (requires CASA approval),
   - tethering inside NFZ of a non-controlled aerodrome (no extra approval, but
     must meet the relevant standard),
   - tethering in restricted/military controlled airspace (requires LOA).
3. **Add identification guidance for aerodrome no-fly zones and operating
   areas** — a description (and ideally figures) showing the black/grey/white
   shaded zones, their dimensions, and the height limits that apply in each.
4. **Add a detailed specialised procedure (Appendix-level)** covering:
   - Height and airspace limitations (tether length cap, height above ARP,
     elevation determination, ATC notification and radio monitoring).
   - A method/formula for calculating the maximum permitted tether length based
     on ground attachment elevation vs aerodrome elevation.
   - Operational documentation and approval requirements (Flight Record, JSA,
     risk assessment addressing controlled-airspace risks, NOTAM submission
     timeline and recipient, CRP approval prior to each operation).
   - Pre-flight, landing, and post-flight checklists specific to the tether
     system.
   - A limitations table (vertical/horizontal speed, wind, lateral
     displacement, flight time reduction, VLOS, NOTAM status).
   - Emergency procedures specific to tethered operations (tether retract
     failure, lost link while tethered, tether system maintenance intervals).
   - Identification of the RPA platform(s) and tether system used (CASA asked for
     this explicitly).
   - Crew requirements: minimum crew (e.g. two for a non-automated tether), crew
     training and CRP approval for tethered operations.
   - Standard phraseology tables for the remote pilot, tether operator and any
     emergency commands.
   - Tethered operations at non-controlled aerodromes and helicopter landing
     sites (MOS 9.05) and at military controlled aerodromes (letter of agreement
     and clearance before take-off).
5. **Submit a significant change application to CASA** with the updated
   Operations Manual, using the correct form (see Section 4 — common pitfall).
6. **Update the Amendment Record** of the Operations Manual to log the change,
   the affected sections, and the approval status.
7. **Prepare for CASA's scenario questionnaire** — after its first review CASA
   may ask you to complete written scenario questions (tether length at example
   sites, no-fly-zone geometry, NOTAMs). See
   [Scenario questionnaire — how to prepare](Scenario%20questionnaire%20-%20how%20to%20prepare.md).

---

## 3. Steps needed (process overview)

1. **Internal decision & scoping** — confirm the operational need for tethering
   inside controlled aerodrome NFZs (e.g. for jobs near Class C/D airspace).
2. **Select an assessor/consultant** (if used) to assist with the ReOC
   amendment.
3. **Review the current Operations Manual** against the checklist in Section 4
   below to identify gaps.
4. **Draft the updated Operations Manual sections** using the template in
   Section 5.
5. **Internal review and sign-off** by the Chief Remote Pilot (CRP) / relevant
   personnel.
6. **Lodge the significant/non-significant change application** with CASA,
   attaching the updated Operations Manual.
   - **Use the correct form** — a significant/non-significant change form, not
     the initial issue/variation/renewal form (this was a real cause of delay).
7. **Respond to CASA feedback** — expect more than one round. CASA may request
   re-lodgement on the correct form, then (once an inspector is assigned) provide
   its template tether procedures and ask you to insert any missing sections and
   complete a written scenario questionnaire. Answer every point in one
   consolidated reply with evidence attached.
8. **Pay any assessment/processing fees** quoted by CASA.
9. **Await CASA assessment outcome** — CASA doesn't send individual progress
   updates (it points applicants to its published service delivery timeframes).
   In the case documented here an inspector was assigned about four months after
   payment; the assessment itself then took about five and a half weeks, with
   written feedback instead of an interview, ending in an approval letter.
10. **On approval**, check the letter names the exact manual version and date you
    submitted (if it differs from your cover page, ask CASA to confirm which
    document was approved rather than editing the accepted file), file the
    letter, update the Amendment Record with the approval date and conditions, and
    brief all relevant pilots/crew on the new procedure before conducting any
    tethered NFZ operations.
11. **Operational use** — for each planned tethered NFZ operation: complete
    Flight Record/JSA/risk assessment, submit NOTAM within the required
    timeframe, confirm CRP approval, confirm NOTAM active, and proceed per the
    new appendix procedure.

---

## 4. How to review your current ReOC and map out what needs adding

Use this checklist to compare your existing Operations Manual against what's
required for tethering in NFZ approval.

| # | Item to check in current manual | Gap if missing |
|---|----------------------------------|-----------------|
| 1 | Does the "Operations near aerodromes" / no-fly zone section explain the black/grey/white zone shading, dimensions, and applicable height limits? | Add an "Identification of Aerodrome No-Fly Zones and Operating Areas" subsection with figures/diagrams. |
| 2 | Does the "Tethered operations" policy section distinguish between tethering outside NFZ, inside NFZ of a controlled aerodrome, inside NFZ of a non-controlled aerodrome, and in restricted/military airspace? | Rephrase/expand the tethering policy section to cover all four scenarios separately, with correct approval requirements for each. |
| 3 | Is there a statement that CASA approval is specifically required for tethered ops in the NFZ of a controlled aerodrome? | Add explicit statement and cross-reference to the new specialised procedure appendix. |
| 4 | Is there a statement covering non-controlled aerodrome NFZ tethering (no extra approval needed if standard met) and relevant-event allowances? | Add/confirm this statement. |
| 5 | Is there a statement covering restricted/military controlled aerodrome airspace requiring an LOA? | Add this statement if your operations could occur near such airspace. |
| 6 | Does the specialised procedures appendix for tethering have a dedicated section for "Tethered operations within the no-fly zone of a controlled aerodrome" (separate from general tether requirements)? | Add a new appendix subsection (see template Section 5). |
| 7 | Does that section include a tether length calculation method accounting for ground attachment elevation vs aerodrome elevation? | Add the calculation formula and worked example. |
| 8 | Does it specify ATC notification before take-off and radio monitoring requirements? | Add explicit ATC notification/monitoring requirements. |
| 9 | Does it specify the documentation chain (Flight Record, JSA, risk assessment) addressing controlled-airspace-specific risks before applying for CASA approval? | Add documentation requirements. |
| 10 | Does it specify NOTAM submission — who submits, how far in advance, and to which address? | Add NOTAM process with lead time and contact details. |
| 11 | Are there pre-flight/landing/post-flight checklists specific to the tether system for NFZ operations? | Add or adapt checklists. |
| 12 | Is there a limitations table (speed, wind, lateral displacement, flight time reduction, VLOS, NOTAM status) specific to NFZ tethered ops? | Add limitations table. |
| 13 | Are there emergency procedures specific to tethered NFZ operations (tether retract failure, lost link while tethered, maintenance intervals)? | Add emergency procedures subsection. |
| 14 | Is the Amendment Record up to date, listing the affected section numbers and a description of the change? | Add a new amendment record row referencing the updated sections. |
| 15 | Is the correct CASA form identified for lodging this as a significant/non-significant change (not an initial issue/variation/renewal form)? | Confirm correct form before lodging — common cause of processing delay. |
| 16 | Does the tethering appendix identify the RPA platform(s) and the tether system used? | Add a "Tether system and components" section naming the RPA and tether (manufacturer, type, automated or manual). CASA asked for this explicitly. |
| 17 | Are minimum crew, crew training and CRP approval for tethered operations stated? | Add crew requirements (e.g. two crew for a non-automated tether; a number of supervised training tethered operations; a theory element on tether length calculation). |
| 18 | Are standard phraseology tables (remote pilot, tether operator, emergency commands) present and consistent with your emergency procedures? | CASA's template is a guide, not a prescribed standard, so optional commands can be left out — but if you include emergency commands, say in the emergency procedures when each one is used. |
| 19 | Does your non-controlled aerodrome / HLS procedure cover all of MOS 9.05(3) and (4)? | Add: 150 ft tether; RPA no higher than 150 ft above aerodrome elevation; grey area, or black area not within 3 NM of a runway measurement point; for HLS at least 465 m from the central axis and VLOS. |
| 20 | Do the numbers in your no-fly-zone description match MOS 4.05 (distances either side of the centreline, 7 km, 8.5 km, 3 NM, 300 ft / 150 ft)? | Cross-check every number against the MOS text, not a figure or an older manual (see the [quick reference](MOS%20clause%20quick%20reference.md)). |
| 21 | Have you compared each section of CASA's template tether procedures with your manual, line by line? | CASA expects you to find and insert missing sections; be ready to explain anything you leave out. |
| 22 | Does your near-people section address work next to buildings (building wash, window cleaning)? | Add a cross-reference and controls (see section 5.5). |
| 23 | After restructuring, are all section numbers, cross-references and Amendment Record entries still correct? | Re-render the document and check each reference. |

**Output of this review:** a list of section numbers in your manual that need
to be added or amended, which becomes your CASA submission's "affected
sections" list (see template amendment record row).

---

## 5. Template — Operations Manual update for Tethering in NFZ

Copy and adapt the sections below into your Operations Manual. Section numbers
are examples — renumber to match your manual's existing structure.

### 5.1 Amendment Record entry (template)

| Amdt No. | Date | Approval status | Affected sections | Description of change |
|---|---|---|---|---|
| [next #] | [date] | To be approved | [e.g. Section 2.4.X — Tethered operations; Appendix D — Tethered operations within the no-fly zone of a controlled aerodrome] | Tethering in no-fly zone approval: [Section 2.4.X] — rephrased general tethering policy to distinguish controlled aerodrome NFZ, non-controlled aerodrome NFZ, relevant events, and restricted/military airspace requirements. [Appendix D.X] — added detailed specialised procedure for tethered operations within the no-fly zone of a controlled aerodrome. |

### 5.2 Policy section — Tethered operations (template)

> ### Tethered operations
>
> The CRP may approve tethered operations.
>
> CASA approval is required for tethered operations in the no-fly zone of a
> controlled aerodrome. Procedures must be conducted in accordance with [the
> specialised procedure in Appendix D.X] and the relevant Part 101 MOS
> provisions.
>
> Tethered operations within the no-fly zone of a non-controlled aerodrome are
> permitted without additional CASA approval, provided they meet the relevant
> Part 101 MOS requirements for non-controlled aerodromes. They are also
> permitted during relevant events.
>
> For tethered operations within restricted airspace at a military controlled
> aerodrome, a valid Letter of Agreement (LOA) permitting tethered operations
> must be obtained from the controlling authority. The operator must ensure
> clearance has been obtained from the controlling authority prior to each
> take-off.
>
> For the specialised tethered operation procedures, refer to Appendix D.

### 5.3 New subsection — Identification of Aerodrome No-Fly Zones and Operating Areas (template)

> #### Identification of Aerodrome No-Fly Zones and Operating Areas
>
> [Insert figure(s) showing the no-fly zone shading for relevant
> aerodromes/airspace.]
>
> For controlled aerodromes, the no-fly zone includes the black-shaded areas
> depicted in the figure. At the runway, the black area is a rectangle extending
> **500 m on either side of the runway centreline** and overlying the runway strip
> (Part 101 MOS 4.05(3)(b)). The approach and departure paths extend from the ends
> of the runway strip, splaying at 15° either side, to **7 km** (black, from the
> ground up) and **8.5 km** (cross-hatched, from 300 ft above aerodrome elevation)
> (MOS 4.05(2) and 4.05(3)(a)). Tethered operations are not permitted in the black
> area within 3 NM of the runway measurement point (MOS 4.04(3)(f)).
>
> The grey area extends 3 NM in all directions from the runway measurement point
> (MOS 4.05(4)). Tethered operations in the grey area are permitted provided the
> tether does not exceed 150 ft, the RPA does not exceed 150 ft above aerodrome
> elevation (MOS 4.04(3)(a) and (b)), and the flight does not breach the Obstacle
> Limitation Surfaces (OLS).
>
> Approval must be sought from CASA for operations at locations higher than these
> procedures allow.

**Common error to avoid.** In the case documented here, the manual that CASA
assessed described the black area as extending "1.5 km either side" of the
runway centreline, and measured the 7 km from the runway threshold. That figure may
have come from a label on the MOS figure. MOS 4.05(3)(b) says **500 m** either side,
and 4.05(2)(b)(i) measures the 7 km from the **end of the runway strip**. The manual
was more conservative than the MOS, not less, and CASA did not raise it — but it
disagreed with the correct scenario answer, so fix it at the next revision. If you
change wording CASA has already accepted, check whether the change is significant
under MOS 10A.01.

### 5.4 New Appendix subsection — Tethered operations within the no-fly zone of a controlled aerodrome (template)

> #### Tethered operations within the no-fly zone of a controlled aerodrome
>
> Tethered operations within the no-fly zone of a controlled aerodrome must be
> conducted in accordance with this Operations Manual. For general tether
> system requirements applicable to all tethered operations, refer to [general
> tether appendix section]. For the overarching approval requirements and
> applicable airspace rules, refer to [tethering policy section].
>
> **Height and airspace limitations**
>
> - The RPIC must ensure the tether does not exceed [length] and that the RPA
>   is not operated above [height] above the Aerodrome Reference Point (ARP)
>   elevation. Where a CASA approval specifies a lower maximum height, the RPA
>   must not be operated above that approved height.
> - Aerodrome elevation must be determined from the Aerodrome Obstacle
>   Limitation Surface (OLS) data or obtained from the ERSA. Site elevation
>   must be confirmed using [mapping tool] and at least one second source prior
>   to each operation, and the RPA height (AMSL) confirmed on site — mapping
>   tools can show different elevations for the same location (CASA noted that
>   Google Earth web and desktop can differ).
> - The RPIC must notify ATC prior to take-off and must operate the RPA in
>   accordance with any instructions issued by ATC. The aviation radio must be
>   monitored at all times during tethered operations to maintain situational
>   awareness of surrounding air traffic.
>
> **Calculating the maximum permitted tether length**
>
> The RPIC must calculate the maximum permitted actual tether length prior to
> each operation using the following method:
>
> - T = permitted actual length of tether
> - a = maximum tether length permitted under the relevant MOS chapter (150 ft: MOS 4.04(3)(a))
> - b = elevation of the tether ground attachment point (AMSL)
> - c = aerodrome elevation (AMSL)
>
> Equation: **T = a − (b − c)**
>
> The result must **not exceed 150 ft**: if the formula gives more than 150 ft
> (the ground attachment point is below the aerodrome elevation), the maximum
> tether length is 150 ft (MOS 4.04(3)(a)).
>
> Example: tether ground attachment point = [value] AMSL; aerodrome elevation
> = [value] AMSL; location in grey area with maximum tether length of [value].
>
> T = [a] − ([b] − [c]) = [result]
>
> Therefore, the maximum length of the tether permissible is [result].
>
> **Operational documentation and approval requirements**
>
> - Tethered operations within the no-fly zone of a controlled aerodrome must
>   not be conducted without prior CASA approval. All operations conducted
>   under this appendix must also be approved by the CRP prior to commencement.
> - Prior to submitting an application for CASA approval, a Flight Record, JSA,
>   and risk assessment must be completed. These documents must address the
>   operational environment, including the presence of low-flying aircraft and
>   risks specific to tethered operations in controlled airspace, and must
>   detail how the conditions of the approval will be met, identifying and
>   mitigating any additional operational risks.
> - The CRP must ensure a NOTAM is submitted for each operation conducted under
>   these procedures. The NOTAM must be forwarded to [contact/email] at least
>   [lead time] prior to the planned operation. The RPIC must confirm the NOTAM
>   is active prior to take-off.
>
> **Pre-flight and post-flight checklists**
>
> The RPIC must ensure that tether system setup and operating procedures are
> conducted in accordance with the manufacturer's checklist or, where no
> manufacturer checklist exists, the operator's internally developed
> procedure. The following is provided as a minimum-standard example and must
> be reviewed and adapted to suit the specific tether system in use.
>
> *Pre-flight, landing and post-flight:*
> - Confirm NOTAM is active.
> - Check serviceability of all tether components.
> - Confirm the site elevation (AMSL) on site against your recorded figure and
>   recalculate the tether length if it differs.
> - Lay out the tether line to the take-off/landing point.
> - Attach tether to RPA and confirm correct attachment by a second,
>   independent inspection.
> - Note the maximum approved height and set the tether to the calculated
>   maximum permitted length.
> - Maintain active listening to the CTAF or ATC involved in the intended
>   tethered operation area. Communicate with ATC or other traffic when the
>   pilot in command determines a need to maintain safety.
> - Proceed on task using standard phraseology as per [reference].
> - [Include any system-specific steps for the tether system in use.]
> - Confirm intention to land with all crew.
> - Commence tether retraction and monitor descent.
> - Announce "hold tether" when the RPA is just above the landing area.
> - Pilot in command to announce when it is safe for crew to approach the RPA
>   after landing.
> - Inspect tether for damage, pack up equipment, and complete the Flight
>   Record.
>
> **Limitations**
>
> The following operational limitations apply to all tethered operations
> within the no-fly zone of a controlled aerodrome. Additional limitations may
> be imposed by the CASA approval or by the CRP. Where a more restrictive
> limitation is specified by the OEM, that limitation applies.
>
> | Parameter | Limitation |
> |---|---|
> | Maximum vertical speed | [value] |
> | Maximum horizontal speed | [value] |
> | Maximum wind speed | OEM maximum wind speed limit applies |
> | Maximum lateral displacement from tether ground point | [value] |
> | Reduction in rated flight time | [value] (or as specified in JSA) |
> | Visual line of sight | Operation must remain within VLOS at all times |
> | NOTAM | NOTAM must be confirmed active prior to take-off |
>
> Note: The limitations above are minimum standards. Operators must review
> these values against the specific RPA, tether system, and site conditions,
> and apply more restrictive limits where required.
>
> **Emergency procedures**
>
> The following emergency procedures apply specifically to tethered
> operations. General emergency procedures are detailed in [general emergency
> section] of this Operations Manual.
>
> *Tether retract unit inoperable*
> - If the tether operator announces "stop stop stop", the RPIC must
>   immediately hold the RPA in a stable position at current height.
> - The tether operator must manually wind in the tether line and control the
>   descent.
>
> *RPA lost link*
> - The RPIC announces "lost link, hold tether". The tether operator must
>   immediately confirm "holding tether" and await further instructions from
>   the RPIC.
> - The RPIC must attempt to re-establish the data link. If the link cannot be
>   re-established within a safe timeframe, the tether operator must manually
>   wind in the RPA.
>
> *Emergency commands (optional)*
> - CASA's template phraseology is a guide, not a prescribed standard. If you
>   include emergency commands in your phraseology table (for example "STOP STOP
>   STOP"), state in this section the circumstances in which each is used and
>   what the crew must do, in the same way as for "Tether retract unit
>   inoperable". Commands you don't need can be left out.
>
> *Tether system maintenance*
> - The tether unit and all components must be inspected before and after each
>   flight.
> - A complete serviceability check of the winding unit and full pay-out of the
>   tether line must be completed every [interval] flights or [interval] hours
>   of tethered operation, whichever occurs first, or more frequently if
>   required by the OEM.
> - All maintenance activities must be recorded in the RPAS Technical Log in
>   accordance with [maintenance section] of this manual. The MC must note any
>   approvals or restrictions specific to the tether system on the maintenance
>   log for the approved system.

### 5.5 Operations next to buildings (building wash / window cleaning) — people near the work (template)

Tethered building-wash and window-cleaning jobs put the RPA close to people:
pedestrians, building occupants and neighbours. CASA asked that the
operations-near-people requirements in the manual be considered and complied
with when planning this work. Cross-reference your near-people section from the
tethering appendix and from the risk assessment. CASA's guidance is on its page
[Flying over and near people](https://www.casa.gov.au/drones/flight-authorisations/flying-over-and-near-people).

> #### Operations adjacent to buildings
>
> When planning tasks adjacent to buildings, including tethered window or façade
> cleaning, the RP must assess the presence and movement of people within 30 m
> laterally of the RPA at every stage of the task, and apply [operations near
> people section]. The RPA must not be flown over any person.
>
> The JSA must record:
>
> - a ground exclusion zone beneath and around the work face, including the area
>   within the tether length, the quadrant downwind of the tether ground point
>   and likely spray drift, controlled with signage, barriers and spotters where
>   needed;
> - the time of day with the lowest foot traffic and, where practicable,
>   temporary closure of nearby entrances and walkways;
> - how people within 30 m will be identified and, where the RPA will operate
>   within 30 m but not closer than 15 m, how each person's written consent will
>   be obtained; and
> - that the RPA will not be operated closer than 15 m laterally to any person
>   not directly associated with the operation, unless the operator holds a CASA
>   approval for it.
>
> The operation must stop, and the RPA be held clear or landed, if a person enters
> the exclusion zone or comes within 15 m.

The CASA page did not say whether people *inside* a building count as people for
these rules, so treat anyone at windows, balconies, entrances or rooftops as
people unless you have assessed otherwise, and record that in the JSA.

---

## 6. Submission checklist (CASA lodgement)

- [ ] Updated Operations Manual with all sections from Section 4 checklist
      addressed.
- [ ] Amendment Record updated with affected section numbers.
- [ ] Correct CASA form used — significant/non-significant change form (not
      the initial issue/variation/renewal form).
- [ ] Flight Record, JSA, and risk assessment templates updated to address
      controlled-airspace-specific risks.
- [ ] NOTAM process documented with correct contact and lead time.
- [ ] Internal sign-off by CRP completed prior to submission.
- [ ] Budget allowance made for CASA processing fee and any
      consultant/assessor fees, payable on receipt of CASA's estimate letter.
- [ ] Scenario questionnaire prepared (see
      [how to prepare](Scenario%20questionnaire%20-%20how%20to%20prepare.md)), with the
      MOS clause cited in every rule-based answer.
- [ ] Every number in the manual and the answers cross-checked against the current
      MOS (4.04, 4.05, 9.05).
- [ ] Elevation figures taken from two sources, and the same figure used in the
      manual, the answers and the evidence.
- [ ] Near-people controls for work next to buildings cross-referenced (section 5.5).
- [ ] After approval: approval letter checked against your manual's version and
      date, then filed.

---

## 7. Notes / lessons learned

- Confirm the correct form **before** first submission — submitting on the
  wrong form (e.g. initial issue/variation/renewal instead of
  significant/non-significant change) causes CASA to request re-lodgement and
  significantly delays the timeline.
- Expect a gap of several weeks to a couple of months between submission and
  CASA's substantive response/fee estimate — factor this into operational
  planning.
- Keep the general tethering policy section and the detailed NFZ appendix
  procedure cross-referenced to each other so reviewers and pilots can navigate
  between the "what's allowed" policy and the "how to do it" procedure.
- CASA doesn't send individual progress updates; it asks applicants not to email
  for status and to use its published service delivery timeframes. In the case
  documented here an inspector was assigned about four months after payment, then
  the assessment took about five and a half weeks in two written feedback rounds.
- Read the inspector's wording exactly. "Please ensure X is considered and complied
  with" is an acknowledgement, not necessarily a request to rewrite the manual, and
  "you may include" means optional.
- CASA's template procedures are a guide, not a prescribed standard — but compare
  every template section with your manual and be able to explain what you left out.
- Put the MOS clause reference beside every number, and take elevations from two
  sources, in the first submission. The second feedback round was entirely about
  evidence.
- Keep numbers identical across the manual, the scenario answers and the evidence,
  and check them against the MOS text rather than a figure or an older manual.
- After restructuring the appendix, re-render the document and check section
  numbers, cross-references and the Amendment Record — they drift.
- A change of company name (same ACN) is a separate application on Form 101-02 and
  the manual must show the current legal entity name. CASA was happy to receive one
  revised manual covering both the admin and the tether changes, as long as the
  revision log shows everything clearly.
- Confirm the approval letter names the exact manual version and date you
  submitted.
