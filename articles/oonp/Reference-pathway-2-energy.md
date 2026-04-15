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

### 1. Protection from laceration

Pathway 2 imposes specific rules about exposed rotating parts (propellers):

### Simple Summary

- **1:1 ratio** → distance from people = height of drone  
- **No exposed props** within that zone  
- **3 m minimum height** when operating close (≤15 m), unless mitigated  

---

***1:1 Ratio - Separation Rule***

Operations within the 1:1 ratio zone, the RPA must **not** have exposed rotating parts that could lacerate human skin.

**1:1 ratio** means:

> The horizontal distance between the RPA and a person must be at least equal to the RPA’s height above that person.

**Acceptable solutions** could be
> Propeller guards (physically cover the blades)
> Parachute Recovery System (PRS) (**stop propeller rotation** when deployed)

For example, if your RPA is at **10 m AGL**, then it has to be at least **10 m horizontally** away from any person. You can't operate closer than 10 m from people, unless the RPA has no exposed rotating parts capable of lacerating human skin. In this case, if you could incorporate a parachute system that stops propeller rotation upon parachute activation, then it is taken to meet this requirement.

***Additional Height Rule (Within 15 m)***

If operating **within 15 m horizontally** of a person, the RPA must be at least **3 m above the person’s height**, unless:
  - The RPA has **no exposed rotating parts**, **or**
  - The RPA has a functional **obstacle avoidance system** that prevents it from coming within 5 m horizontally

---

Solutions:

- **Propeller guards** — physically cover the propellers
- **Parachute Recovery System (PRS)** — must stop propeller rotation upon activation (the TMI states that PRS systems that stop rotation are "taken to meet this requirement")


> **Practical implication:** For most multirotor operations near people at close range, you need either prop guards, ducted propellers, or a reliable obstacle avoidance system.

---

### 2. Speed restriction requirements (If Used as a Mitigation)

Reducing maximum flight speed is the most common method for sub-250 g platforms. If you're using a speed restriction to stay below 15 J (e.g., Cine Mode on a DJI Mini), the following applies:

- The speed restriction **must be set so the pilot cannot exceed it without an intentional override action** (eg. physically switching flight modes). Relying on pilot discipline alone is not sufficient.
- The speed limit must be a **system-enforced** setting, not just a briefing item (flight mode lock, firmware limit).
- In environments where signal interruption is probable (e.g., near buildings), account for the RPA possibly exceeding the restricted speed during autonomous manoeuvres (e.g., RTH)
- **Documented** in the energy calculation with the specific mode and speed cited

---

### 3. Failure mode considerations

Your energy assessment must account for **the most probable failure modes**, including:

- **Loss of GNSS** — especially relevant in urban environments, near tall buildings, or indoors where signal interruption is likely
- **Fly-away scenarios** — what happens if the RPA loses control link?
- **Battery failure** — sudden loss of power at maximum altitude
- **Wind effects** — can wind push the RPA above the speed threshold?

CASA assumes **all kinetic energy is transferred to the person** on impact unless you provide validated evidence of energy absorption (e.g., frangibility data reviewed by CASA's Airworthiness and Engineering Branch).

---

## Energy Reduction Methods

There are a few ways to keep the energy level below the threshold.

### Parachute recovery systems

A parachute compliant with **ASTM F3322-18** can be used to reduce terminal velocity and bring the RPA below the energy threshold. If the parachute stops propeller rotation on deployment, it also satisfies the laceration requirement.

### Sheltering

Sheltering uses a structure or barrier to physically protect people from impact. Requirements:

- RPA ≤ 25 kg
- Operations must be in a controlled environment (no possibility of a person exiting the shelter during operations). People inside a building (behind glass, under a roof) may be considered **sheltered**, they are protected by the structure and do not need to be active participants
- The operator must declare the shelter construction is sufficient. If the RPA penetrated the structure, the residual energy transfer is below the permitted maximum.
- A person is **sheltered in a vehicle only if the vehicle is enclosed** (e.g. cars, trucks, not motorcycle).
- **Moving vehicles are considered sheltered only when travelling below 50 km/h, or when the driver has provided informed consent.**

---

## Consent Under Pathway 2 (15–34 J)

If your RPA exceeds 15 J but stays within 34 J, you can still use Pathway 2, but you need **informed consent** from the persons you're operating near.

Pathway 2 consent is deliberately **lighter** than Pathway 1 (with fewer formal requirements). The energy is lower, so the risk profile is lower. But "lighter" doesn't mean "casual", you still need a documented, repeatable process.

### Pre-consent briefing

Before consent is given, the operator's personnel must brief each consenting person on:

1. The **proposed RPA flight paths** — where the drone will fly relative to them
2. The **risk to life** — including details of potential injury probability and severity. At 15–34 J, the risk of serious injury exists but fatality is unlikely. Be honest and specific — don't minimise, but don't overstate either.
3. **Emergency procedures** and the emergency response plan — what happens if something goes wrong, and what the person should do
4. **Safety mitigations** implemented to control harm and risk — speed restrictions, observer, access control, etc.
5. Their **right to not consent** — participation must be voluntary and unpressured

> **Note:** Compare this to Pathway 1's briefing, which includes two additional briefing items: the 30 m separation rule disclosure and the explicit fatality statement for >34 J energy. Those aren't required here because Pathway 2 consent applies only in the 15–34 J range, which is below the fatality threshold.

### Key differences from Pathway 1 consent

| Aspect | Pathway 1 | Pathway 2 (15–34 J) |
|---|---|---|
| **Consent format** | Must be written and signed | No written requirement — verbal acceptable if documented |
| **Briefing items** | 6 items (includes 30 m rule and fatality statement) | 5 items (no 30 m rule or fatality statement — energy is below that threshold) |
| **Age limit** | 18+ only, no exceptions | No age limit — guardian can consent for minors |
| **Proxy consent** | Not permitted | Permitted by legal guardian |
| **Capacity check** | Required | Required — plus documented procedure for minors/reduced capacity |
| **Who can brief** | Must have appropriate experience | Must have appropriate experience |
| **Withdrawal** | Should be permitted | Should be permitted |

> **Important:** Operations involving minors or persons with reduced capacity carry a **higher risk profile**. The TMI explicitly requires the operator to have a documented procedure addressing this.

> **Note on TMI language:** The TMI uses "should" (not "must") for several Pathway 2 consent items: documented procedures, capacity methods, recording consent. That's softer language than Pathway 1's "must." But in practice, if CASA might expect to see all of these addressed. Treat the "should" items as requirements for the purposes of your manual, it's much easier to document them upfront than to explain their absence during an audit.


### How consent is obtained

Unlike Pathway 1, there is **no requirement for written consent** under Pathway 2. However, the TMI states the operator should have documented practices and procedures that detail:

- **How persons will be adequately briefed** prior to providing informed consent
- **How consent was obtained** — verbal consent is acceptable, but you need a record of it
- **Who can deliver the briefing** — personnel must hold appropriate experience to ensure the briefing is adequate

**Practical options for recording consent:**

| Method | When it works | Considerations |
|---|---|---|
| **Verbal consent with witness** | Small groups, informal settings (e.g., wedding party) | Record the person's name, time, who witnessed, and that the briefing was delivered |
| **Verbal consent recorded on a sign-in sheet** | Events, group briefings | Person signs or initials next to their name after the verbal briefing |
| **Written consent form** (voluntary) | Higher-risk operations, commercial clients who expect paperwork | Not required by the TMI, but provides stronger evidence of compliance |
| **Audio/video recording of briefing and consent** | Large groups where individual signatures are impractical | Ensure privacy requirements are met |

> **Tip:** Even though written consent isn't mandatory, having *something on paper* makes your life easier if CASA audits you or if there's an incident. A simple sign-in sheet with a printed statement and signature line is low-effort and high-value.

### Capacity and eligibility

- **Age:** There is **no age limit** under Pathway 2 consent. A legal guardian can consent on behalf of a minor (under 18). This is a significant difference from Pathway 1, where minors are excluded entirely.
- **Proxy consent:** Permitted — a legal guardian can consent on behalf of a minor or a person who lacks capacity.
- **Capacity:** Adults are assumed to have capacity, but the operator must have a method to ensure consent is not accepted from a person lacking capacity. If a person lacks capacity, consent must be obtained from their legal guardian. A person with capacity will understand and retain the information, understand the choices and consequences, weigh them up, and communicate a decision freely and voluntarily.
- **Minors and reduced capacity:** The TMI explicitly states that operations involving minors or persons with reduced capacity have a **higher risk profile**. Your Operations Manual must include a documented procedure addressing how you manage these situations — it's not enough to just say "guardian can consent."

---

**Example procedure for minors:**

> Where a minor (under 18) is present within the Pathway 2 operational area and impact energy exceeds 15 J, the following applies:
>
> 1. The minor's legal guardian must be present on site
> 2. The guardian receives the standard Pathway 2 briefing
> 3. The guardian is informed that they are consenting on behalf of the minor
> 4. The guardian's consent is recorded (name of guardian, name of minor, relationship, time)
> 5. The CRP assesses whether additional mitigations are warranted (e.g., increased separation distance, additional observer attention to the minor's location)

### Withdrawal of consent

A person (or their guardian) should be able to withdraw consent at any time. Your procedures should address:

- How a person signals they want to withdraw (tells crew, leaves the area)
- Whether operations pause or the RP adjusts the flight path to maintain separation
- How the withdrawal is recorded

> **Practical reality:** At events, people move in and out of the operational area constantly. Your procedures should account for the fact that "consent" at an event is often tied to a person's voluntary presence in a briefed area, rather than a locked-in commitment. If someone moves away, that's effectively withdrawal — and if they come back, a re-brief may be needed.

### Record retention

Consent records (whether written forms, sign-in sheets, or notes of verbal consent) should be stored securely and retained for the period specified in your CASA approval instrument. If no period is specified, retain for at least **12 months** as a minimum good practice — this aligns with typical CASA data collection and reporting requirements for OONP operations.

---

## Fleet Energy Register

For each RPA and configuration used in OONP operations, you need a completed **energy worksheet** filed in a Fleet Energy Register. This should include:

- RPA model and serial number
- Configuration (standard battery, extended battery, accessories, parachute)
- Total mass in each configuration
- Permitted flight modes for OONP and the maximum speed for each mode
- Calculated total energy (kinetic + potential energy)
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









