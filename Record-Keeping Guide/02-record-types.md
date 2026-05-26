# 02 — Record Types

This section breaks down every record type a ReOC holder needs to maintain. For each type, we explain what it is, what must be included, who keeps it, how long to keep it, and a practical example.

> **Important:** This guide covers ReOC operator records only. RePL training provider record-keeping requirements (MOS 101 s10.09 onwards) are a separate, complex topic and are not covered here.

Last reviewed: 18 April 2026

---

## How Records Are Grouped

The MOS 101 Chapter 10 can feel overlapping at first. To make them manageable, it helps to group records by **function** rather than by section number. Here's how they break down into three logical groups:

| Group | What It Covers | MOS 101 Sections |
|---|---|---|
| **A. Operational Records** | Everything related to planning, authorising, flying, and documenting an operation | s10.03, s10.04, s10.05 |
| **B. Personnel & Training Records** | Everyone who works under your ReOC and what training they've received | s10.03(2), s10.08 |
| **C. RPA & Pilot Records** | The aircraft's maintenance/techcnical and the pilot's personal flight log | s10.06, s10.07 |

This grouping reduces overlap and makes filing practical. A single operation generates records in Group A. When you train someone, it goes in Group B. Aircraft maintenance sits in Group C.

---

> **Note on excluded RPA (Division 10.3):**  
> This guide is intentionally written around the **full record-keeping framework for certified ReOC operations** under **MOS 101 Division 10.2 (RPA other than excluded RPA)**.
>
> CASA provides a **simplified record-keeping regime for excluded RPA operations** under **Division 10.3**, which generally has:
> - fewer mandatory fields
> - shorter retention periods for some records (for example, 3 years for the operational log)
> - no operational release requirement in the same form as a ReOC operation
>
> In practice, if your operation may involve both excluded and certified/ReOC activities, it is often simpler and better from a compliance and audit perspective to **use the full record set in this guide for all operations**.  
> Doing so avoids having to manage two separate rule sets and ensures records remain consistent across different job types.

---

## Group A: Operational Records

### A1. General Operational Documents — s10.03(1)

**What it is:** MOS 101 s10.03(1) requires the CRP to keep supporting documents that sit alongside the operational release and log for every operation.

**What must be included:**

| Document | MOS 101 Reference | Notes |
|---|---|---|
| Job Safety Analysis (JSA) | s10.03(1)(a) | Site-specific hazard identification and controls |
| Risk Assessment (RA) | s10.03(1)(b) | May not be required for every operation, Check your ops manual |
| Operational Flight Plan | s10.03(1)(c) | If issued for the operation |

**Who keeps and how long:** CRP and 7 years from the date of creation.

**Practical example:** You fly a roof inspection job at a school. Before the flight, you complete a JSA identifying overhead power lines, pedestrian traffic, and a nearby helipad. You also complete a risk assessment because the site is near a restricted area. Both documents are saved as PDFs named `mission001_JSA_20260415.pdf` and `mission001_RA_20260415.pdf` and filed alongside the operational record.

> **Tip:** The provided Operations Record template includes document tracking columns (JSA on file, RA on file, Flight plan on file) to cross-reference these documents against each operation. This is a simple way to prove that the documents exist and are filed correctly.

---

### A2. RPAS Operational Release — s10.04

**What it is:** The operational release is the **pre-flight authorisation**. It is the documented record that the operation has been reviewed, the RPA is serviceable, the crew is assigned, and the person with authority has approved the flight to proceed.

Think of it as a "cleared to operate" document. It must be completed **before** the operation commences.

**What must be included:**

| Field | MOS 101 Reference | Description |
|---|---|---|
| Nature and purpose of the operation | s10.04(a) | What you're doing and why |
| RPA type, model, and unique ID | s10.04(b) | Which aircraft, identified by your internal registration |
| Remote pilot station location | s10.04(c) | Where the RP will be standing/operating from |
| Date of operation | s10.04(d) | When the operation is planned |
| Launch location, recovery location, max height AGL | s10.04(e) | Where you're flying from/to and how high |
| Name and ARN of remote pilot(s) | s10.04(f) | PIC and any additional RPs |
| Names and roles of non-RP crew | s10.04(g) | Observers, ground handlers, etc. |
| Whether VLOS, EVLOS, or BVLOS | s10.04(h) | Type of visual line of sight |
| Whether CASA approvals are held | s10.04(i) | Any specific CASA instruments or exemptions |
| RPA serviceability confirmed | s10.04(j) | The aircraft is fit to fly — confirmed by the maintenance controller |
| Release approved by | s10.04(2) | Name of the person authorising the operation |

**Sole operator exception:** If the ReOC holder is the only remote pilot operating under the ReOC, the "release approved by" field is not required (s10.04(5)).

**Who keeps and how long:** CRP and 7 years from the date of creation.

**Practical example:** Before a solar panel cleaning job, the PIC (or CRP) completes the pre-flight columns of the Operations Record spreadsheet: date, purpose, aircraft ID, location coordinates, crew details, VLOS type, serviceability confirmed, and release approved. This happens before the drone leaves the ground.

---

### A3. RPAS Operational Log — s10.05

**What it is:** The operational log is the **post-flight record**. It documents what actually happened during the operation. MOS 101 s10.05 requires the PIC to complete this as soon as practicable after the flight.

**What must be included:**

| Field | MOS 101 Reference | Description |
|---|---|---|
| Actual dates and times | s10.05(d) | When the operation actually took place |
| Flight segments and heights | s10.05(j) | What was actually flown, including any time above 400ft AGL |
| Whether RPA became unserviceable | s10.05(k) | Did the aircraft develop a fault during the operation? |
| Log completed by (PIC) | s10.05(f) | The PIC signs off the post-flight record |

**Key MOS 101 note:** The operational log can simply confirm "no changes from release" if the operation proceeded exactly as planned. You don't need to re-document everything, just note any deviations.

**Who keeps and how long:** CRP and 7 years from the date of creation.

**Practical example:** After the solar panel cleaning job, the PIC returns and completes the post-flight columns of the same row in the Operations Record: actual times 0900–1045, "flight as per release, max 25m AGL," RPA serviceable throughout, log completed by [PIC name].

---

### How A2 and A3 Work Together

The operational release and operational log are two sides of the same coin: one is "before," one is "after." In the provided template, they share the same row. Each operation gets one row, and the pre-flight and post-flight sections are completed at different times.

This combined approach avoids duplicate data entry and makes it easy to see the full lifecycle of each operation in one place.

---

## Group B: Personnel & Training Records

### B1. Personnel Records — s10.03(2), s10.08, reg 101.342(b)

**What it is:** The personnel register is a master record of every person who operates under your ReOC:  remote pilots, observers, ground handlers, loading staff, and anyone else with a safety-related role. It records their qualifications, induction status, type training, operator approvals, and current/inactive status.

ReOC holder needs to maintain a record of the qualifications of each person who performs duties for the operator. MOS 101 s10.08 requires that non-RP crew (observers, ground handlers, loading staff) are trained to perform their duties safely and that records of this training are kept.

**What must be included (at minimum):**

| Field | Source Reference | Description |
|---|---|---|
| Full name | s10.03(2), reg 101.342(b) | Legal name of the person |
| ARN | reg 101.342(b) | Aviation Reference Number (for RPs) |
| Role | reg 101.342(b) | Their role under the ReOC (RP, SRP, observer, etc.) |
| Contact details | Operational necessity | Phone, email, address |
| Flight experience | reg 101.342(b) | Hours by category (multirotor, fixed wing, etc.) |
| Qualifications | reg 101.342(b) | RePL held, IREX/BVLOS status |
| Induction status | Best practice / ops manual | Whether induction training is complete |
| Type training | s10.03(2)(c) | Training on specific RPA types they are authorised to fly |
| Operator approvals | Ops manual | Night, EVLOS, Senior RP, tethering, etc. |
| Non-RP training | s10.08 | Observer, ground handler, loading staff training status |
| Current or inactive | Administrative | Whether the person is currently active under the ReOC |
| Dates commenced and ceased | s10.03(2) | When they started and stopped operating under the ReOC |

**Who keeps and how long:** CRP and 7 years from the date of creation.

**Practical example:** When a new remote pilot joins your operation, you add them to the Personnel Register with their details, check and record their qualifications, note their flight experience, record their induction date, and track which aircraft types they're trained on. When they leave, you mark them "inactive" and note the end date. You keep the record for another 7 years.

---

### B2. Training Log — s10.03(2)

**What it is:** A record of all **internal training** (non-RePL) conducted under the ReOC. This includes induction training, type ratings, competency assessments, observer/ground handler training, recurrent training, and any other training activity managed by the CRP.

MOS 101 s10.03(2) requires the CRP to keep a record of the training given to each person. The record must include specific details about the when, what, and outcome of the training.

**What must be included:**

| Field | MOS 101 Reference | Description |
|---|---|---|
| Trainee identity | s10.03(2)(a) | Full name and ARN of the person being trained |
| When the training took place | s10.03(2)(b) | Date(s) of training |
| Nature, extent, and purpose | s10.03(2)(c) | What kind of training (assessment, under instruction, observation), what it covered, and what it was for |
| Result of the training | s10.03(2)(d) | Pass, fail, or in progress |

**Additional practical fields (recommended):**

| Field | Purpose |
|---|---|
| Trainer name and ARN | Who delivered the training |
| Location | Where the training took place |
| RPA type and model | Which aircraft was used (if applicable) |
| Duration | How long the training took |
| Ops approvals granted | Any privileges awarded as a result (e.g. "EVLOS approved") |
| Assessment form on file | Whether a formal assessment record exists |
| CRP sign-off | CRP acknowledges the record |

**Who keeps and how long:** CRP and 7 years from the date of creation.

**Practical example:** You train a new remote pilot on your DJI M400 over two sessions. Session 1 is a ground/theory day covering type-specific procedures. Session 2 is a practical flight assessment. Each session gets its own row in the Training Log: TR-001 and TR-002. The entries record who was trained, by whom, when, what was covered, the outcome, and the CRP sign-off.

---

### How B1 and B2 Work Together

The Personnel Register is the **snapshot** — who is qualified for what right now. The Training Log is the **history**: what training has been delivered over time.

When someone completes training (logged in B2), their Personnel Register entry (B1) gets updated to reflect their new qualifications or approvals. The two records cross-reference each other.

---

## Group C: Aircraft & Pilot Records

### C1. Remote Pilot Log — s10.06

**What it is:** The remote pilot log is a personal flight record maintained by each individual remote pilot. It records their flying history, hours, and types flown. It's similar in concept to a manned aircraft pilot logbook.

MOS 101 s10.06 specifies what must be recorded. Note that the remote pilot log is the **pilot's** record, not the organisation's, but the CRP should ensure that pilots are maintaining their logs.

**What must be included:**

| Field | MOS 101 Reference | Description |
|---|---|---|
| Date of flight | s10.06 | When the flight took place |
| RPA type and model | s10.06 | What aircraft was flown |
| Location | s10.06 | Where the flight occurred |
| Duration | s10.06 | How long the flight was |
| Type of operation | s10.06 | VLOS, EVLOS, BVLOS; day or night |
| Role | s10.06 | PIC, co-pilot, or under instruction |
| Cumulative totals | s10.06 | Running total of flight hours |

**Who keeps and how long:** CRP and 7 years from the date of creation.

**Practical tip:** Many pilots use the DJI flight log or similar app-generated data as a starting point, but this alone is generally not sufficient. The pilot log should be a structured record that includes the fields above. A simple spreadsheet works well.

> **Relationship to the Operational Log:** The remote pilot log and the operational log (A3) capture overlapping information but serve different purposes. The operational log is an **organisational** record of the operation. The pilot log is a **personal** record of the pilot's flight history. They should be consistent with each other, but they are maintained separately.

---

### C2. RPAS Technical Log — s10.07

**What it is:** The RPAS technical log is the **aircraft's service and maintenance record**. It tracks the status, maintenance, defects, and serviceability of each airframe. Think of it as the aircraft's health record.

MOS 101 s10.07 requires a technical log for each RPA. The level of detail may vary based on the complexity of the aircraft and the operations being conducted, but every aircraft used under the ReOC should have one.

**What must be included:**

| Field | MOS 101 Reference | Description |
|---|---|---|
| RPA identification | s10.07 | Type, model, serial number, and your internal unique ID |
| Flight hours / cycles | s10.07 | Running total of operational time |
| Maintenance actions | s10.07 | What maintenance was performed, when, and by whom |
| Defects and rectifications | s10.07 | Any faults found and how they were addressed |
| Serviceability status | s10.07 | Is the aircraft currently fit to fly? |
| Component replacements | s10.07 | Propellers, batteries, motors, etc. with dates and hours |
| Firmware/software updates | Best practice | Record of software and firmware versions |

**Who keeps it:** The maintenance controller (MC) or CRP, depending on your ops manual structure and 7 years from the date of creation.

**Practical example:** Your DJI M400 has a technical log that records every flight cycle, battery swap, propeller replacement, firmware update, and any defect. After 50 flight hours, you replace the propellers: this goes in the technical log with the date, hours at replacement, and part details.

> **Relationship to the Operational Release:** The serviceability confirmation in the operational release (s10.04(j)) is linked to the technical log. Before each operation, the maintenance controller (or whoever holds that responsibility) confirms the aircraft is serviceable based on the technical log.

---

## Reducing Overlap

One of the biggest frustrations operators have with MOS 101 is that the requirements can feel repetitive. The operational release, operational log, pilot log, and technical log all capture information about the same flight.

The key is to understand that each record serves a **different purpose**:

- The **operational release** proves the flight was authorised.
- The **operational log** proves the flight was conducted and completed safely.
- The **pilot log** tracks the individual pilot's experience.
- The **technical log** tracks the aircraft's lifecycle.

The provided templates reduce this overlap by combining the operational release and operational log into a single row-per-operation spreadsheet. This means you only enter aircraft and crew details once, then complete the post-flight section in the same row. Similarly, the Personnel Register and Training Log share a single workbook, so qualification updates flow naturally from training events.

---

**Next:** [03 — Implementation Guide](03-implementation-guide.md) — how to set up your record-keeping system in practice.
