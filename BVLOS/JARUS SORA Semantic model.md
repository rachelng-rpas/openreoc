# SORA Semantic Model

**Author: Rachel Ng | 26 May 2026**

🔗 [JARUS guidelines on Specific Operations Risk Assessment (SORA)](http://jarus-rpas.org/wp-content/uploads/2024/06/SORA-v2.5-Main-Body-Release-JAR_doc_25.pdf)

---

## Ground Risk Volumes

| Layer | Components |
|-------|-----------|
| Intrinsic GRC footprint | Area to which the operation needs to be contained: Operational Volume + Risk Buffer |
| Operational Volume | Flight geography + Contingency volume |
| Beyond operational volume | Risk buffer + Adjacent area |

## Air Risk Volumes

| Layer | Components |
|-------|-----------|
| Airspace to consider for ARC | Airspace to which the operation needs to be contained: Operational Volume |
| Operational Volume | Flight geography + Contingency volume |
| Beyond operational volume | Adjacent airspace |

---

## Operation Control States

The SORA considers two states of the operation: in control and loss of control.

| | In control | In control | Loss of control |
|---|---|---|---|
| **State** | Normal operation | Abnormal situation (undesired state) | Emergency situation (unrecovered state) |
| **Response** | Standard operational procedures | Contingency procedures (return home, manual control, land on a pre-determined site, etc.) | Emergency procedures (land asap or activation of FTS, etc.) |
| **Plan** | | | Emergency response plan (plan to limit escalating effect of the loss of control of the operation) |

**In control** — remote crew can manage the flight without putting anyone on the ground or in the air in immediate danger.

- **Normal operation**: follows standard operating procedures.
- **Abnormal situation**: standard procedures no longer work, but no one is in immediate danger. Safety margins are reduced. Crew must execute contingency procedures to return to normal or safely end the flight.

**Loss of control** — outcome relies on providence, or the situation can't be handled by contingency procedures. Includes: UA exits operational volume, UA doesn't follow the predefined route and can't be controlled, UA crashes, or unplanned flight termination is triggered (even inside the operational volume).

- **Emergency procedures**: executed by remote crew (may be supported by automated features like FTS). Aim to either return to an in-control state or minimise hazards until flight ends. Should activate as soon as UA reaches the operational volume boundary, or earlier if recovery is clearly impossible (e.g. loss of propulsion).
- **ERP**: deals with secondary/escalating effects after loss of control (e.g. emergency services response). Does not deal with controlling the UA itself.
- **Containment**: technical and operational mitigations to keep the UA within the operational volume and ground risk buffer and reduce likelihood of a flyaway.
