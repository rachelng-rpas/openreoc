# OONP Pathway Selection Matrix & Practical Applications

> **Purpose:** This document combines the **Pathway 1 vs Pathway 2 selection framework** with **real-world operational examples** to support consistent decision-making under CASA TMI 2024-01.

---

## Contents

- [OONP Pathway Selection Matrix](#oonp-pathway-selection-matrix)
- [Step 1 — Environment Gate](#step-1--environment-gate)
- [Step 2 — Pathway 1 Eligibility Check](#step-2--pathway-1-eligibility-check-controlled-environment)
- [Step 3 — Pathway 2 Eligibility Check](#step-3--pathway-2-eligibility-check-energy-based-operations)
- [Final Selection Logic](#final-selection-logic)
- [Practical Examples](#practical-examples)
- [Sheltering — How It Works With Pathway 1](#sheltering--how-it-works-with-pathway-1)

---

# OONP Pathway Selection Matrix

> **Purpose:** This matrix provides a single decision framework to determine whether **Pathway 1 (Controlled Environment)** or **Pathway 2 (Energy-Based Operations)** applies to an OONP mission under CASA TMI 2024-01.

---

## Step 1 — Environment Gate

| Question | YES | NO |
|---|---|---|
| Can you physically control access to the entire operational area (including ground risk buffer)? | Go to Pathway 1 | Go to Pathway 2 |
| Are all persons within the area either RPA crew or active participants? | Go to Pathway 1 | Go to Pathway 2 |

> If **YES to both**, Pathway 1 may apply.  
> If **NO to either**, Pathway 2 must be used (if energy limits allow).

---

## Step 2 — Pathway 1 Eligibility Check (Controlled Environment)

Use Pathway 1 only if ALL conditions are satisfied:

- [ ] Can every active participant be individually briefed and sign consent?
- [ ] Are all active participants ≥ 18 years old?
- [ ] Is the RPA ≤ 25 kg?
- [ ] Do you hold a current ReOC?
- [ ] Have you assessed whether a populous area exemption (reg 101.280) is also required?

### Pathway 1 Decision

- If **ALL YES → Pathway 1 APPROVED**
- If **ANY NO → Pathway 1 NOT PERMITTED → consider Pathway 2**

---

## Step 3 — Pathway 2 Eligibility Check (Energy-Based Operations)

Use Pathway 2 only if ALL conditions are satisfied:

- [ ] Have you completed an energy calculation for this specific RPA + configuration?
- [ ] Is total impact energy (worst credible case) ≤ 15 J (no consent) or ≤ 34 J (with consent)?
- [ ] Is speed restriction system-enforced (not pilot discipline)?
- [ ] Does the RPA comply with laceration protection requirements?
- [ ] Have you assessed failure modes (GNSS loss, fly-away, battery failure)?
- [ ] Is required consent obtained (if operating 15–34 J)?
- [ ] Is the energy calculation filed in the Fleet Energy Register?
- [ ] Is the OONP Pre-Flight Checklist updated?
- [ ] Have you assessed whether a populous area exemption (CASR 101.280) is required?

### Pathway 2 Decision

- If **ALL YES → Pathway 2 APPROVED**
- If **ANY CRITICAL NO → Pathway 2 NOT PERMITTED**

---

## Final Selection Logic

| Situation | Approved Pathway |
|---|---|
| Fully controlled environment + all Pathway 1 criteria met | **Pathway 1** |
| Uncontrolled or mixed environment + energy compliant | **Pathway 2** |
| Energy > 34 J | **Neither Pathway 1 nor 2 → Pathway 3 (SORA required)** |

---

## Practical Examples

---

### Example 1 — Building Exterior Wash

**Scenario:** Washing a 6-storey residential building. Occupied, with pedestrians on an adjacent footpath.

- **Controlled environment**
  - Ground-level barriers (cones, tape, fencing) around the building base  
  - Observer positioned at access points  

- **Active participants**
  - Ground crew, building management representative, observer, remote pilot  
  - All provide written consent  

- **Building occupants**
  - Remain inside with windows closed → considered **sheltered**  
  - No consent required (notification recommended)  

- **Public interface (footpath)**
  - If closed → include within controlled environment  
  - If not → **Pathway 1 does not apply** above that area  
    - Consider **Pathway 2** or adjust timing  

- **Operation**
  - Wash drone operates ~3 m from façade within controlled area  

---

### Example 2 — Closed Film Set

**Scenario:** Filming inside a warehouse studio (15 crew, 3 actors).

- **Controlled environment**
  - Enclosed warehouse with restricted access (locked doors)  

- **Active participants**
  - All persons inside are briefed and provide written consent  

- **Operation**
  - Drone flies over actors for overhead shots  
  - Permitted under Pathway 1  

- **Risk mitigation**
  - Propeller guards or PRS recommended when operating within 1:1 ratio  

---

### Example 3 — Construction Site Inspection

**Scenario:** Inspection of a building under construction.

- **Controlled environment**
  - Existing site controls (fencing, gates, sign-in procedures)  

- **Active participants**
  - Workers within the operational area are briefed and consented  
  - Site manager confirms access control  

- **Operation**
  - Drone operates near workers performing inspection tasks  

---

### Example 4 — Private Property Shoot

**Scenario:** Real estate filming at a private residence.

- **Controlled environment**
  - Defined property boundary (fenced or naturally bounded)  

- **Active participants**
  - Client and assistants provide written consent  

- **External persons (neighbours)**
  - Not part of the controlled environment  
  - If operating near boundary:
    - Obtain consent; or  
    - Maintain separation; or  
    - Apply Pathway 2 if suitable  

---

## Sheltering — How It Works With Pathway 1

Sheltering allows certain people to be **not treated as exposed**, reducing the need for consent.

### Common Scenarios

| Scenario | Status | Consent Required |
|----------|--------|-----------------|
| Inside building (windows closed) | **Sheltered** | No |
| On open balcony | **Not sheltered** | Yes (or exclude) |
| Under solid awning | Case-by-case | Operator assessment |
| Inside parked, enclosed vehicle | **Sheltered** | No |
| On motorcycle / unenclosed vehicle | **Not sheltered** | Yes (or exclude) |

---

### Practical Implication

For building operations:

- Occupants inside with windows closed → **sheltered**
- Do **not** require consent  
- Only personnel **within the controlled environment** require consent  

> Always notify occupants via building management to prevent unexpected exposure (e.g. opening windows or entering balconies).
