# RPAS Terminology & Definitions Bank

Author: Rachel Ng

Last updated: 3 June 2026

---

Plain English definitions of regulatory and operational terms. Include the actual regulatory reference where possible.

---

| Term | Definition (Plain English) | Regulatory Reference |
|------|---------------------------|----------------------|
| iGRC | Intrinsic ground risk class — the risk level on the ground before any safety measures are applied | AusSORA / SORA 2.5 |
| fGRC | Final ground risk class — the risk level on the ground after safety measures like sheltering or impact reduction are applied | AusSORA / SORA 2.5 |
| ARC | Air risk class — rates how likely the drone is to encounter other aircraft, based on airspace type | AusSORA / SORA 2.5 |
| AEC | Airspace encounter category — classifies the type of airspace and likelihood of running into manned aircraft | AusSORA / SORA 2.5 |
| SAIL | Specific assurance and integrity level (1–6) — the higher the number, the stricter the safety requirements for drone, training, and risk management | AusSORA / SORA 2.5 |
| Integrity | Quality of the safety objective — how well designed and implemented it is | SORA 2.5 OSO |
| Assurance | Level of confidence that a safety objective will actually be achieved | SORA 2.5 OSO |
| Robustness | Combines integrity and assurance into one rating — optional, low, medium, or high. Characteristics of risk mitigation / OSOs (level of integrity + level of assurance) | SORA 2.5 OSO / JARUS SORA 2.5 |
| OSO | Operational safety objective — specific safety goals that manage risks if the drone goes out of control | AusSORA / SORA 2.5 |
| ConOps | Concept of operations — the document describing what you're doing, where, how, and what could go wrong | AusSORA Step 1 |
| Containment | Managing risk in the adjacent area if OSOs fail — operation expected to end if loss of control goes beyond the ground risk buffer | AusSORA Step 6 |
| ERP | Emergency response plan — how local authorities (fire, ATC) will respond if the drone is out of control | AusSORA Step 7 |
| M1 | Sheltering mitigation — reduces ground risk by accounting for structures that protect people on the ground | AusSORA GRC |
| M2 | Impact reduction mitigation — reduces ground risk through design features like parachutes or frangibility | AusSORA GRC |
| **UAS Operational Category A (Open)** | Low risk. Minimal regulatory involvement. No mandatory airworthiness — operator self-certifies. Safety managed through operational limitations like VLOS and location restrictions. Operator is responsible for safe operations. | JARUS SORA 2.5 - 2.5.1 |
| **UAS Operational Category B (Specific)** | Goes beyond Open limitations but not high enough for full certification. Authority independently assesses via risk assessment (e.g. SORA). Mitigations can include design requirements, operational limits, and pilot qualifications. Varying oversight levels — authority issues operational approval. *This is where most BVLOS work sits.* | JARUS SORA 2.5 - 2.5.2 |
| **UAS Operational Category C (Certified)** | High unmitigated risk. Full regulatory oversight like manned aviation. Requires type certification, certificate of airworthiness, flight manuals, production approvals. Risk can't be managed by operational limitations alone. | JARUS SORA 2.5 - 2.5.3 |
| TLOS | Target Level of Safety — defined for people and aircraft uninvolved in the operation; commensurate with existing manned aviation levels of safety to the same stakeholders | JARUS SORA 2.5 |
| Flight geography | For normal operation, RPA should only operate inside this volume. Can be a corridor or an area covering multiple changing flight paths. The boundary should include margins for system and operational errors (deviation, error, latency, etc.) | JARUS SORA 2.5 |
| Contingency volume | Surrounds the flight geography. Entering this volume is considered an abnormal situation requiring contingency procedures to return to the flight geography. | JARUS SORA 2.5 |
| Operational volume | = Flight geography + Contingency volume. It is where the operation is intended to take place. Together with the ground risk buffer, it protects the adjacent area and airspace. If the RPAS leaves the operational volume, emergency procedures must be activated immediately. | JARUS SORA 2.5 |
| Ground risk buffer | Surrounds the contingency volume. If the UA exits the contingency volume during an emergency, the flight must end within the ground risk buffer. **(a) Initial ground risk buffer** is defined either: (i) using the **1:1 principle** — 1 ft of buffer per 1 ft of AGL operating altitude; or (ii) a **different value proposed by the applicant** using the principles in Annex E, Section E.4, Criteria 3. **(b) The final ground risk buffer may differ from the initial one** in cases such as: (i) medium or high level of containment; or (ii) use of ground risk mitigations, such as a parachute. Size is based on individual risk of operation, UA characteristics, and containment requirements. | JARUS SORA 2.5 |
| Controlled ground area | The intended UAS operational area where **only involved persons (if any) are present** — i.e., a level of assurance that no uninvolved persons will be in the operational area. Controlled ground areas are a way to strategically mitigate ground risk. Ensuring area control is the **full responsibility of the operator**; the authority may request evidence of how control will be maintained (e.g. physical barriers, access control, signage, entry briefings, no public rights of way). | JARUS SORA 2.5 / AU-STS |
| Adjacent area | Ground area adjacent to the ground risk buffer. The inner limit starts at the outer limit of the ground risk buffer; the outer limit starts from the inner limit of the ground risk buffer. | JARUS SORA 2.5 |
| Adjacent airspace | Airspace adjacent to the operational volume. | JARUS SORA 2.5 |
| Ground risk class | Determined by the operational volume + ground risk buffer. | JARUS SORA 2.5 |
| Ground Risk | Determined by the population density within the operational volume and ground risk buffer. Applicants must use ABS data to determine population density in adjacent surrounding areas. A controlled ground area requires documented practices showing how the flight area is managed if any unexpected person or vehicle enters. | AU-STS |
| Air Risk | The operational volume must be in atypical airspace. If adjacent areas include Class C or D airspace or military CTR, an air risk buffer must be applied. BVLOS within the relevant airspace of an uncontrolled aerodrome must be shielded with aerodrome radio frequencies monitored. Operations within Class C/D airspace or military CTRs require consultation with Airservices Australia or the controlling Defence unit where above 400 ft AGL, in approach/departure paths, or within 3 NM of the movement area. | AU-STS |
