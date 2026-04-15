# VERY FIRST DRAFT, DO NOT REFER TO YET

# OONP Pathway 2 — Energy-Based Operations (Unlikely to Cause Serious Harm)

> **Understanding CASA's TMI 2024-01 Pathway 2 for Operations Over or Near People**
>
> **Last updated:** 15 April 2026
> 
> **Regulatory basis:** TMI 2024-01, CASR 101.245, CASR 101.280, CASA EX45/24, Direction 7 of CASA 22/22

---

## Contents



---

## What Is Pathway 2?

Pathway 2 authorises RPA operations **over or near people, including uninvolved persons**, where the RPA's potential **impact energy transfer does not exceed 15 joules**. The 15 J threshold is the point below which CASA (drawing on JARUS/EASA research) considers impact **unlikely to cause serious harm**.

Unlike Pathway 1, you **do not need a controlled environment** and you **do not need consent** from overflown persons (at the ≤15 J level). 

This makes Pathway 2 the go-to pathway for operations where members of the public may be present and cannot be excluded: events, public spaces, occupied buildings, and similar environments.

---
## Quick Decision Checklist

Use this before selecting Pathway 2 for a mission:

- [ ] Have you completed an energy calculation for this specific RPA + configuration?
- [ ] Is the total impact energy (horizontal + vertical, worst credible case) ≤ 15 J (no consent) or ≤ 34 J (with consent)?
- [ ] Is speed restriction system-enforced (not relying on pilot discipline)?
- [ ] Have you assessed failure modes (GNSS loss, fly-away, battery failure)?
- [ ] Does the RPA comply with laceration protection requirements at the planned proximity?
- [ ] If operating 15–34 J: have you obtained informed consent and documented it?
- [ ] Have you assessed whether a populous area exemption (reg 101.280) is also required?
- [ ] Is the energy calculation filed in the Fleet Energy Register?
- [ ] Is the OONP Pre-Flight Checklist updated for this configuration?

---

## Understanding Impact Energy

### What is "impact energy"?

Impact energy is the **kinetic energy the RPA would transfer to a person** on impact. Think of it as a measure of "how hard the drone hits."

The formula is straightforward:

```
Kinetic Energy (joules) = ½ × mass (kg) × velocity² (m/s)
```

A drone's total impact energy is usually a **combination of**:

- **Vertical kinetic energy (/potential energy)** — from falling (gravity + descent speed)
- **Horizontal kinetic energy** — from forward flight speed

Both components must be considered together, because a drone doesn't just fall straight down, it also has forward momentum.

---

## Energy Thresholds Summary

| Threshold | Consent required? | Conditions |
|---|---|---|
| **≤ 15 J** | No | Base Pathway 2 — no consent needed from overflown persons |
| **≤ 34 J** | Yes (informed consent) | Pathway 2 with consent — verbal briefing + recorded consent (written not mandatory but recommended) |
| **≤ 34 J** | No | Emergency services operations conducted **by** an emergency services organisation only |
| **> 34 J** | — | Cannot use Pathway 2 — use Pathway 1 (controlled environment) or Pathway 3 (SORA) |

---

### Example energy calculations

| RPA | Mass | Speed | Approx. kinetic energy | Within 15 J? |
|---|---|---|---|---|
| DJI Mini (standard) | 0.249 kg | 6 m/s (Cine Mode) | ~4.5 J | Yes |
| DJI Mini (standard) | 0.249 kg | 16 m/s (Sport Mode) | ~32 J | **No** |
| Sub-2 kg filming drone | 0.8 kg | 6 m/s | ~14.4 J | Marginal — verify |
| Sub-25 kg wash drone | ~15 kg | Any speed | Far exceeds 15 J | **No** — use Pathway 1 |

> **Note:** These are simplified horizontal-only examples. Your actual energy calculations must include vertical energy from the RPA's altitude and terminal velocity, plus account for failure modes. Expect to show the worst-case credible scenario, not the best-case normal flight.

---

## When to Use Pathway 2 vs Pathway 1

| Factor | Pathway 1 | Pathway 2 |
|---|---|---|
| **Uninvolved persons present?** | No — all persons are consented active participants | Yes — members of the public may be present |
| **Environment** | Fully controlled (barriers, access control) | Uncontrolled or partially controlled |
| **Energy limit** | None (up to 25 kg RPA) | ≤ 15 J without consent; ≤ 34 J with consent |
| **Consent** | Written informed consent from every person | Not required at ≤ 15 J |
| **Typical use** | Closed worksites, film sets, wash operations | Events, public spaces, occupied buildings |
| **RPA size** | Up to 25 kg | Practically limited to sub-250 g or sub-2 kg platforms at low speed |

**Hybrid approach:** Many real-world operations combine both pathways. For example, a building wash may use Pathway 1 for the barricaded site (consented crew) and Pathway 2 for the buffer zone near a public footpath — provided the wash drone's energy profile permits.

---

## Operational Limitations and Requirements

### Protection from laceration

Pathway 2 imposes specific rules about exposed rotating parts (propellers):

- **Within a 1:1 ratio** (horizontal distance ≤ height above person): The RPA must **not** have exposed rotating parts that could lacerate skin. This means if your drone is 10 m high and 10 m horizontally from a person, exposed props are prohibited.
- **Within 15 m horizontal but less than 3 m above a person**: Prohibited unless:
  - The RPA has **no exposed rotating parts** (e.g., ducted fans), **or**
  - The RPA has a functional **obstacle avoidance system** that prevents it from coming within 5 m horizontally

> **Practical implication:** For most multirotor operations near people at close range, you need either prop guards, ducted propellers, or a reliable obstacle avoidance system.

### Speed restriction requirements

If you're using a speed restriction to stay below 15 J (e.g., Cine Mode on a DJI Mini):

- The speed restriction **must be set so the pilot cannot exceed it without an intentional override action** (such as switching flight modes). Relying on pilot discipline alone is not sufficient.
- The speed limit must be a **system-enforced** setting, not just a briefing item.

### Failure mode considerations

Your energy assessment must account for **the most probable failure modes**, including:

- **Loss of GNSS** — especially relevant in urban environments, near tall buildings, or indoors where signal interruption is likely
- **Fly-away scenarios** — what happens if the RPA loses control link?
- **Battery failure** — sudden loss of power at maximum altitude
- **Wind effects** — can wind push the RPA above the speed threshold?

CASA assumes **all kinetic energy is transferred to the person** on impact unless you provide validated evidence of energy absorption (e.g., frangibility data reviewed by CASA's Airworthiness and Engineering Branch).

---

## Energy Reduction Methods

### Parachute recovery systems

A parachute compliant with **ASTM F3322-18** can be used to reduce terminal velocity and bring the RPA below the energy threshold. If the parachute stops propeller rotation on deployment, it also satisfies the laceration requirement.

### Speed restrictions

Reducing maximum flight speed is the most common method for sub-250 g platforms. The restriction must be:

- **System-enforced** (flight mode lock, firmware limit)
- **Not easily overridden** during flight without deliberate action
- **Documented** in the energy calculation with the specific mode and speed cited

### Sheltering

Sheltering uses a physical structure to protect people from impact. Requirements:

- RPA ≤ 25 kg
- Operations must be in a controlled environment (no possibility of a person exiting the shelter during operations)
- The shelter must ensure residual energy from any penetration is below the permitted maximum
- **Moving vehicles** are not shelter unless travelling < 50 km/h, or the driver has given informed consent

---

## Consent Under Pathway 2 (15–34 J)

If your RPA exceeds 15 J but stays within 34 J, you can still use Pathway 2, but you need **informed consent** from the persons you're operating near.

### Briefing requirements (before consent)

The operator's personnel must brief each consenting person on:

1. The proposed RPA flight paths
2. Risk to life, including potential injury probability and severity
3. Emergency procedures and the response plan
4. Safety mitigations in place
5. Their right to refuse consent

### Key differences from Pathway 1 consent

| Aspect | Pathway 1 | Pathway 2 (15–34 J) |
|---|---|---|
| **Consent format** | Must be written | No written requirement (but document how consent was obtained) |
| **Age limit** | 18+ only | No age limit — guardian can consent on behalf of a minor |
| **Proxy consent** | Not permitted | Permitted by legal guardian |
| **Capacity check** | Required | Required — operator must have a documented method |

> **Important:** Operations involving minors or persons with reduced capacity carry a **higher risk profile**. The TMI explicitly requires the operator to have a documented procedure addressing this.

---

## Fleet Energy Register

For each RPA and configuration used in OONP operations, you need a completed **energy worksheet** filed in a Fleet Energy Register. This should include:

- RPA model and serial number
- Configuration (standard battery, extended battery, accessories, parachute)
- Total mass in each configuration
- Maximum speed in the restricted flight mode
- Calculated kinetic energy (horizontal + vertical components)
- Permitted flight modes for OONP
- Any failure-mode energy calculations
- Date of calculation and sign-off by CRP

New RPA or configurations must have energy calculations completed **before** the first OONP operation.

---

## Operations Manual Requirements

Your Operations Manual must document:

- **Energy calculation methodology** — how you calculate impact energy, what assumptions you use, what failure modes you consider
- **Fleet Energy Register** — a maintained register of energy calculations for each RPA and configuration
- **Pathway Selection Matrix** — how the CRP determines the applicable pathway for each mission
- **Speed restriction procedures** — which flight modes are approved, how the restriction is enforced
- **Laceration protection** — how you comply with the rotating parts requirements
- **Consent procedures** (if operating 15–34 J) — briefing process, how consent is obtained and recorded
- **OONP Pre-Flight Checklist** — confirming energy-related settings before each flight
- **OONP Mission Report** — post-flight record for each OONP operation

---

## Common Mistakes

- **Calculating energy with horizontal speed only.** You must include vertical kinetic energy from the RPA's altitude. A drone at 50 m AGL falling at terminal velocity has significant vertical energy even at zero horizontal speed.
- **Ignoring failure modes.** CASA expects your energy calculation to cover the worst credible scenario, not just normal flight. If GNSS loss could cause a fly-away at Sport Mode speed, that's your energy figure — not Cine Mode.
- **Using Cine Mode but not verifying it's system-enforced.** If the pilot can accidentally bump the mode switch mid-flight and go to full speed, the energy calculation must use full speed.
- **Assuming Pathway 2 means "no rules."** You still need an observer, documented procedures, risk assessments, and CASA approval. The energy threshold replaces consent, not safety management.
- **Forgetting the populous area exemption.** Just like Pathway 1, if you're operating in a populous area, you still need an exemption under regulation 101.280(2). The OONP approval covers regulations 101.245 and Direction 7 — not 101.280.
- **Not recalculating when accessories change the mass.** Adding a parachute, extended battery, or prop guards changes the mass and therefore the energy figure.

---

## Related Resources

- [CASA TMI 2024-01 — RPA Operations Over or Near People](https://www.casa.gov.au) (full text)
- CASR Part 101 — Unmanned Aircraft and Rockets
- ASTM F3322-18 — Standard Specification for sUAS Parachutes
- EASA MOC Light-UAS.2512-01 — M2 Means of Compliance
- JARUS SORA Package (JAR_doc_09)

---

*This guide is part of the [OpenReOC](https://github.com/rachelng-rpas/openreoc) project — open-access CASA ReOC guidance for Australian RPAS operators.*











### 4. Minimum Height

An RPA operated within **15m horizontally** of a person must not be operated at a height **less than 3m** above the height of the person.

**Exceptions:** this restriction may not apply if:
- The RPA has **no exposed rotating parts**, OR
- The RPA has a **functional obstacle avoidance system** that restricts it from operating within 5m of a person

### 5. 1:1 Ratio and Exposed Rotating Parts

Within the 1:1 ratio zone: no exposed rotating parts that could lacerate skin (or PRS that stops props on deployment).

### 6. Speed Restrictions (If Used as a Mitigation)

If speed restrictions are claimed as a safety mitigation:
- Must be set to **prevent the pilot from exceeding** the restricted speed without an **intentional overriding action** (e.g., a physical mode switch)
- In environments where signal interruption is probable (e.g., near buildings), account for the RPA possibly exceeding the restricted speed during autonomous manoeuvres (e.g., RTH)
- 


-
### Sheltering

> The use of a structure or barrier to physically segregate a person from an RPA.

Key points:

- People inside a building (behind glass, under a roof) may be considered **sheltered** — they are protected by the structure and do not need to be active participants
- The operator must declare the shelter construction is sufficient — if the RPA penetrated the structure, the residual energy transfer would not be harmful
- A person in a vehicle is **not** sheltered if: the vehicle is not enclosed (e.g., motorcycle), or the vehicle is travelling over 60 km/h
- Vehicles under 50 km/h where the driver has provided informed consent are considered suitable shelter

### 1:1 Ratio

The **horizontal distance** from the RPA to a person must be at least equal to the **height** of the RPA above ground level.

| RPA Height (AGL) | Minimum Horizontal Distance from Person |
|-------------------|----------------------------------------|
| 5m | 5m |
| 10m | 10m |
| 15m | 15m |
| 20m | 20m |
| 30m | 30m |

This applies within the operational area, even for consenting active participants.

### Exposed Rotating Parts

Operations near people within the 1:1 ratio must **not** occur with an RPA that has exposed rotating parts capable of lacerating human skin.

Solutions:

- **Propeller guards** — physically cover the propellers
- **Parachute Recovery System (PRS)** — must stop propeller rotation upon activation (the TMI states that PRS systems that stop rotation are "taken to meet this requirement")

---

## Sheltering — How It Works With Pathway 1

Sheltering is particularly relevant for **building operations** (washing, inspections) where occupants are inside the structure.

### How Sheltering Interacts with Pathway 1

| Scenario | Persons Status | Consent Needed? |
|----------|---------------|----------------|
| Building occupants inside with windows closed | **Sheltered** — protected by building structure | **No** — notification recommended but consent not required |
| Building occupants on an open balcony | **Not sheltered** — exposed to the RPA | **Yes** — must be an active participant with express written consent, OR must not be in the controlled environment |
| Pedestrians under a solid awning/overhang | Potentially sheltered (depends on construction) | Operator must assess and declare adequacy |
| People in a parked car (enclosed, stationary) | **Sheltered** | No consent required |
| People on a motorcycle | **Not sheltered** | Must be excluded or consented |

### Practical Implication for Building Operations

For building wash or inspection operations, if building occupants have been **notified** to close windows and stay inside, they are **sheltered** and do not need to be active participants. This dramatically reduces the consent burden — you only need express written consent from the people physically outside in the controlled environment (your crew, building management rep, etc.).

> 💡 **Tip:** Always notify building occupants via building management even though consent from sheltered persons is not required. This is good practice and prevents occupants from opening windows or going onto balconies during operations.




