# still DRAFTING, DO NOT FULLY REFERENCE YET

# Step 03 — Amending Your Operations Manual for OONP Approval

A step-by-step guide for ReOC holders to review and amend their RPAS Operations Manual for an OONP (Operations Over or Near People) approval under CASA TMI 2024-01.

> 
> **Last updated:** 7 May 2026

---

## Prerequisites

Before starting, make sure you have:

- [ ] A current ReOC with the RPA you intend to use for OONP listed
- [ ] A copy of [CASA TMI 2024-01](https://www.casa.gov.au) — read it end to end at least once
- [ ] Your current Operations Manual open and editable
- [ ] A clear understanding of what operations you need OONP for and which pathway applies — if you haven't thought this through yet, work through the operational planning considerations in [Step 02 — ConOps](./step-02-conops.md) first. A ConOps is not formally required by CASA but the thinking process is essential before you start amending your manual.
- [ ] Access to your RPA specifications (weight, flight modes, max speeds) for energy calculations

---

## Phase 1 — Gap Analysis

Before writing anything, audit your existing manual against TMI 2024-01. This prevents duplication and identifies exactly what needs to change.

### Method

1. **Keyword search** your manual for: `OONP`, `over or near`, `near people`, `101.245`, `101.280`, `TMI`, `pathway`, `controlled environment`, `active participant`, `energy`, `joule`, `consent`, `populous`, `sheltering`, `Direction 7`, `CASA 22/22`, `CASA 20/25`

2. **For each TMI requirement**, mark your manual:
   - ✅ **Existing** — already covered, quote the section
   - ⚠ **Partial** — present but incomplete, note what's missing
   - ❌ **Gap** — not present at all

3. **Group your findings** into: Pathway 1 requirements, Pathway 2 requirements, and supporting systems (training, emergency, consent, records)

> **Common finding:** Most manuals cover the standard 30–15 m consent under CASR 101.245(3) but have nothing for OONP-approved operations under 101.245(5). Your existing 30–15 m content stays — the OONP content is additional.

---

## Phase 2 — Amendments

Work through your manual in document order. Each section below tells you what to add, where, and which TMI requirement it satisfies.

---

### 2.1 Glossary and Definitions

**TMI reference:** Table 1 (Acronyms), Table 2 (Definitions)

**Add to your acronym table:**

AIS, GNSS, JARUS, OONP, OSO, SAIL, SORA, TMI, and any others from TMI Table 1 not already in your manual.

**Add to your definitions table:**

| Term | Source |
|---|---|
| Active participant | TMI Table 2 — note the scope is deliberately broader than "directly associated with the operation" under CASR 101.245 |
| Controlled environment | TMI Table 2 — requires both exclusion of non-participants AND access control |
| Sheltering | TMI Table 2 |
| Emergency services operation | TMI Table 2 |
| Emergency services organisation | TMI Table 2 |

> **Why this matters:** CASA assessors will check that your manual uses these terms consistently and correctly. Defining them upfront avoids ambiguity throughout the rest of the document.

---

### 2.2 Record Keeping

**TMI reference:** Section 7 (Data collection and reporting requirements)

**Add to your flight records retention table:**

| Record type | Retention period | Notes |
|---|---|---|
| OONP consent record (Pathway 1 and Pathway 2) | Align with your existing standard (typically 7 years) | Separate from standard 30–15 m consent records |
| Fleet Energy Register | 7 years after the RPA was last used in OONP operations | Standing reference document, not per-mission |

**Add a note** explaining the distinction between standard consent records (CASR 101.245(3)) and OONP consent records (TMI 2024-01), and that OONP mission data is captured within the standard flight record.

---

### 2.3 Training

**TMI reference:** Section 3 (Pathway 1 — operator must define personnel and training), Section 4.4 (Pathway 2 — briefer qualification)

**Add an OONP training section** covering:

- All crew (RP, observers, ground support, briefers) must complete OONP training before being assigned to OONP operations
- Reference to your OONP training syllabus (build this in the appendix — see 2.9 below)
- Annual evaluation requirement
- CRP records training in individual training records

Keep it short — the detail lives in the training syllabus appendix.

---

### 2.4 Main Body — OONP Regulatory Framework

This is the most important structural amendment. It establishes when OONP applies and points readers to the detailed procedures.

**TMI reference:** Sections 1.2 (Background — regulatory instruments), 3 (Pathway 1), 4 (Pathway 2)

**Add a new subsection** under your existing "Operations near people" section. Your existing 30–15 m content stays unchanged. The new subsection covers:

**Boundary statement** — operations within 15 m of a person, or directly over any person, require an OONP approval and must not be conducted under standard 101.245(3) consent.

**Regulatory basis** — reference the instruments that govern OONP:
- CASR 101.245(5) — the approval provision
- Direction CASA 20/25 — replaced the expired CASA 22/22 Direction 7, introduces the "safety zone" concept
- CASA EX45/24 (as amended) — provides automatic exemption from populous area requirements (CASR 101.280(2) and 101.250(1)(b)) when you hold an OONP approval. No separate populous area application needed.
- CASA TMI 2024-01 — the policy framework

**Pathway summary:**
- Pathway 1 — controlled environment, written consent, RPA ≤ 25 kg
- Pathway 2 — impact energy ≤ 15 J (or ≤ 34 J with consent)

**CRP authority** — no RP may conduct OONP without CRP authorisation.

**Cross-reference** to your OONP procedures appendix for detailed requirements.

> **Note on CASA 22/22:** TMI 2024-01 was written in April 2024 and references Direction 7 of CASA 22/22. This instrument expired 31 March 2025 and was replaced by Direction CASA 20/25. Your manual should reference 20/25, not 22/22.

**Also add a cross-reference note** under your populous area section pointing back to the OONP section for how populous area requirements are handled under EX45/24.

---

### 2.5 OONP Procedures Appendix

This is the core of your amendment — a dedicated OONP appendix containing all operational procedures. Structure it as follows:

#### 2.5.1 Scope and Applicability

**TMI reference:** Sections 1.2, 1.3

State what operations these procedures apply to (within 15 m, directly over, within safety zone without consent) and what they don't apply to (standard 30–15 m consent, fully enclosed indoor operations). Note that the pathway is determined by conditions, not operation type, and must be recorded in mission planning documentation.

#### 2.5.2 Pathway 1 — Informed Consenting Active Participants

**TMI reference:** Section 3

Cover each requirement from TMI Section 3:

**Controlled environment** — must physically prevent third-party entry using barriers, fencing, cones, signage, or a combination. Must be monitored throughout. *(TMI: "controlled environment" definition)*

**Consent requirements** — written consent from every active participant before operations. Must be 18+. Cannot consent on behalf of another person. *(TMI Section 3, para 1-3)*

**Verbal briefing** — the TMI specifies six items that must be covered verbally before consent is given *(TMI Section 3, bullet list)*:
1. 30 m separation is normally required
2. Energy > 34 J poses significant risk of serious injury or fatality
3. Proposed flight paths
4. Emergency procedures and response plan
5. Safety mitigators in place
6. Right not to consent

**Written declaration** — must state the participant was briefed, accepts risks including fatality, agrees to comply with RP instructions. *(TMI Section 3, para after bullets)*

**Capacity assessment** — adults assumed to have capacity, but briefer must not accept consent from someone lacking capacity. TMI defines capacity criteria. *(TMI Section 3, final note)*

**Briefer qualification** — define who can deliver the briefing and their required training. *(TMI Section 3, note on operator responsibilities)*

#### 2.5.3 Pathway 2 — Unlikely to Cause Serious Harm Upon Impact

**TMI reference:** Section 4

**Energy compliance** — maximum 15 J impact energy demonstrated through calculation of likely impact trajectories including abnormal situations. All kinetic energy assumed transferred unless evidence provided otherwise. *(TMI Section 4, para 1-2)*

**Laceration protection** *(TMI Section 4.1)*:
- No exposed rotating parts within 1:1 ratio (same horizontal and vertical distance)
- Within 15 m horizontal: must not fly below 3 m above person height unless no exposed parts or functional obstacle avoidance within 5 m

**Speed restrictions** *(TMI Section 4.2)*:
- Must be firmware-enforced (no intentional override without mode change)
- Energy assessment must consider probable failure modes including GNSS loss

**Sheltering** *(TMI Section 4.3)*:
- RPA ≤ 25 kg
- No potential for person to exit shelter during ops
- Residual energy through shelter must be below threshold
- Moving vehicles: < 50 km/hr or driver consent

**Parachute systems** *(TMI Section 4.2)*:
- Must comply with ASTM F3322-18 if used
- Optional, not mandatory

#### 2.5.4 Pathway 2 — Consent Procedures (15–34 J)

**TMI reference:** Section 4.4

When informed consent is obtained, the energy threshold increases to 34 J. Cover:

- Five briefing items (different from Pathway 1's six) *(TMI Section 4.4, bullet list)*
- No written consent required, but must document method and record
- Consent may be given by legal guardian — no age limit *(TMI Section 4.4, note on minors)*
- Higher risk profile for minors/reduced capacity — document additional mitigations
- Capacity assessment requirements
- Briefer qualification

#### 2.5.5 Fleet Energy Register

**TMI reference:** Section 4 (energy demonstration requirement)

A standing reference document recording each RPA configuration's energy profile. Must include: RPA details, MTOW, flight modes and max speeds, calculated impact energy, applicable threshold, operating limitations.

**Energy calculation method:**
- Total energy = KE horizontal (½mv²) + PE vertical (mgh)
- Build an impact energy lookup table per configuration: rows = speed, columns = height, cells = total energy in joules
- Colour code: green (≤ 15 J), amber (15–34 J), red (> 34 J)

No RPA may be used in Pathway 2 until its energy calculations are completed, verified, and recorded.

> **Practical tip:** Build the lookup table in a spreadsheet first. The RP uses it during mission planning — pick flight mode (fixes max speed), read across to operating height, confirm you're within threshold. This makes energy compliance a 5-second check rather than a calculation in the field.

#### 2.5.6 Observer Requirements

**TMI reference:** TMI does not mandate observers. Your manual should reflect your operational decision.

If you use observers, define: pre-mission briefing items, positioning, communication protocols, standard calls, and the rule that observers must not be given duties that reduce situational awareness.

#### 2.5.7 OONP Pre-Flight Checklist Supplement

**TMI reference:** Section 3 (Pathway 1 conditions), Section 4 (Pathway 2 conditions)

Additional checks before any OONP flight, covering: pathway selected and recorded, CRP authorisation obtained, energy register verified (P2), consent completed, controlled environment established (P1), crew briefed, comms checked, flight mode set.

#### 2.5.8 OONP Emergency Procedures

**TMI reference:** Implicit in all pathways — operator must have documented emergency procedures.

Cover scenarios specific to OONP:
- Unauthorised person entering operating area
- RPA malfunction or flyaway during OONP
- Loss of energy compliance or separation
- Imminent collision risk with a person

#### 2.5.9 Mission Reporting and CASA Data Requirements

**TMI reference:** Section 7 (Data collection and reporting)

OONP mission reports recorded in the standard flight record with additional fields: pathway used, RPA configuration, number of persons, consent confirmation, any incidents or deviations. CASA reporting per the approval instrument conditions.

---

### 2.6 Consent Forms

**TMI reference:** Section 3 (Pathway 1 written consent), Section 4.4 (Pathway 2 consent record)

Create two separate OONP consent forms:

**Pathway 1 form** — operation details, the six TMI briefing items as a printed declaration, consent and signature table (18+ only, individual signatures).

**Pathway 2 form** — operation details, the five TMI briefing items, consent method (individual verbal / group verbal / guardian), acknowledgement table with name, role, and "consenting on behalf of" column for guardian situations, briefer/RP declaration and sign-off.

> **Keep your existing standard consent form** (30–15 m under CASR 101.245(3)) as a separate document. It serves a different purpose and should not be merged with the OONP forms.

---

### 2.7 Training Syllabus

**TMI reference:** Section 3 (operator must define training for briefing personnel), Section 4.4 (briefer qualification)

Create two training syllabi:

**RP syllabus** — elements and performance criteria covering: regulatory framework, controlled environment, energy compliance, observer duties, emergencies, mission administration. Include practical assessment (simulated OONP operation) and theory knowledge assessment (topic-by-topic).

**Observer / ground support / briefer syllabus** — lighter version covering: understanding the operation, monitoring the area, communication protocols and standard calls, emergency actions, consent and briefing procedures (for briefer-qualified personnel).

---

### 2.8 Approval Instrument

Reserve a section in your appendices for the OONP approval instrument and any associated exemption. Mark it as reserved — CASA will issue this once approved, and it gets filed here.

---

## Phase 3 — Final Check

Before submitting, verify:

- [ ] All internal cross-references are correct (appendix numbers, section numbers, form numbers)
- [ ] TMI definitions in your glossary match TMI Table 2 exactly
- [ ] Pathway 1 briefing has six items matching TMI Section 3
- [ ] Pathway 2 briefing has five items matching TMI Section 4.4
- [ ] Fleet Energy Register has at least one completed entry for the RPA you're applying with
- [ ] Version control table documents all OONP amendments
- [ ] Table of contents page numbers are updated
- [ ] Regulatory references are current: CASA 20/25 (not expired 22/22), EX45/24 (as amended)
- [ ] Your existing standard operations content (30–15 m, populous area) is unchanged and still correct

---

## Submission

Submit to CASA via email to the RPAS team:

- **Operations Manual** (amended version with OONP supplement)
- **CASA multipurpose application form** (Form 101) requesting OONP approval under TMI 2024-01

Internal documents that support your operations but do not need to be submitted:
- Energy calculation spreadsheets (the Fleet Energy Register in the manual is sufficient)
- Consent form templates (CASA can see these in your appendices)
- ConOps (useful for your own planning but not formally required)

---

## Quick Reference — TMI Section Map

| Your manual section | TMI 2024-01 section |
|---|---|
| Definitions | Table 1, Table 2 |
| OONP regulatory framework | Section 1.2 |
| Pathway 1 procedures | Section 3 |
| Pathway 2 procedures | Section 4 |
| Pathway 2 laceration | Section 4.1 |
| Pathway 2 speed/energy reduction | Section 4.2 |
| Pathway 2 sheltering | Section 4.3 |
| Pathway 2 consent (15–34 J) | Section 4.4 |
| Emergency services exemption | Section 4.5 |
| Fleet Energy Register | Section 4 (energy demonstration) |
| Mission reporting | Section 7 |
