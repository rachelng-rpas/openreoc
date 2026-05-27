# RPAS Terminology & Definitions Bank

Author: Rachel Ng

Last updated: 26 May 2026

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
| Robustness | Combines integrity and assurance into one rating — optional, low, medium, or high | SORA 2.5 OSO |
| OSO | Operational safety objective — specific safety goals that manage risks if the drone goes out of control | AusSORA / SORA 2.5 |
| ConOps | Concept of operations — the document describing what you're doing, where, how, and what could go wrong | AusSORA Step 1 |
| Containment | Managing risk in the adjacent area if OSOs fail — operation expected to end if loss of control goes beyond the ground risk buffer | AusSORA Step 6 |
| ERP | Emergency response plan — how local authorities (fire, ATC) will respond if the drone is out of control | AusSORA Step 7 |
| M1 | Sheltering mitigation — reduces ground risk by accounting for structures that protect people on the ground | AusSORA GRC |
| M2 | Impact reduction mitigation — reduces ground risk through design features like parachutes or frangibility | AusSORA GRC |
| **UAS Operational Category A (Open)** | Low risk. Minimal regulatory involvement. No mandatory airworthiness — operator self-certifies. Safety managed through operational limitations like VLOS and location restrictions. Operator is responsible for safe operations. | JARUS SORA 2.5 - 2.5.1 |
| **UAS Operational Category B (Specific)** | Goes beyond Open limitations but not high enough for full certification. Authority independently assesses via risk assessment (e.g. SORA). Mitigations can include design requirements, operational limits, and pilot qualifications. Varying oversight levels — authority issues operational approval. *This is where most BVLOS work sits.* | JARUS SORA 2.5 - 2.5.2 |
| **UAS Operational Category C (Certified)** | High unmitigated risk. Full regulatory oversight like manned aviation. Requires type certification, certificate of airworthiness, flight manuals, production approvals. Risk can't be managed by operational limitations alone. | JARUS SORA 2.5 - 2.5.3 |
| TLOS | Target Level of Safety - defined for people and aircraft uninvolved in the operation and is commensurate with existing manned aviation levels of safety to these same stakeholders | JARUS SORA 2.5|
| Flight geography | For normal operation, RPA should only operate inside this. Can be a corridor or an area covering multiple changing flight paths. The boundary should include margins for system and operational errors (deviation, error, latency etc) | JARUS SORA 2.5 |
| Contingency volume | Surrounds the Flight geography. Entering this volume is considered an abnormal situation, it requires excuting contingency procedures to return to the flight geography. | JARUS SORA 2.5 |
| Operational volume | = Flight geography + Contingency volume. It is where the operaiton is intended to take place. This with the ground risk buffer protect the adjacent area and airspace. If the RPAS leaves the operational volume, emergency procedures must be activated immediately | JARUS SORA 2.5 |
| Ground risk buffer | Surrounds the Contingency volume. If exited the contingency voume during emergencym must end flight within the groud risk buffer. Size is based on individual risk of operation and RPA characteristic and contaiment requirements of SORA | JARUS SORA 2.5 |
| Adjacent area | Ground area adjacent to the ground risk buffer. The adjacent area inner limit starts sat the outer limit of ground risk buffer, the outer limit of the adjacent area starts from inner limit of the ground risk buffer. | JARUS SORA 2.5 |


| Ground risk class | Determined by the Operational volume + ground risk buffer. | JARUS SORA 2.5 |
| Ground Risk | A controlled ground area is defined as an operational area that only involves active participants (if any), and there is a level of assurance that there will be no non-active participants in the area. Applicants will need to detail how the area is controlled, for example: • Control of access by personnel or electronic means. • Physical barrier such as fencing. • Entry control briefing conducted. • Signage in place. • No public rights of way through the area etc. While a 1:1 buffer is not a requirement for all RPA operations utilising this AU-STS, applicants should consider those items set out in section 4.3 Containment to ensure the contingency area will be adequate in providing appropriate separation to adjacent ground areas. The operational volume and the ground risk buffer must be wholly within a controlled ground environment. The applicant must have documented practices and procedures that detail how BVLOS operations are planned and show how the flight operational area is managed if any unexpected person or vehicle enters the controlled area. The applicant must detail the expected active participants in: • the Operational Volume (Flight Geography and Contingency) • any ground risk buffer (if applied). The applicant must show population density by using Australian Bureau of Statistics (ABS) data to determine the population density in adjacent surrounding areas | AU-STS |
| Air Risk | The operation volume must be in atypical airspace. If adjacent areas are class C or D airspace or military CTR, an air risk buffer must be applied. If the applicant requests BVLOS operations within the relevant airspace of an uncontrolled aerodrome, this part of the operation must be shielded, and aerodrome radio frequencies monitored with radio calls being made as required. If shielded operations are not possible, the operations in the relevant airspace of an uncontrolled aerodrome or in the vicinity of a controlled aerodrome must be conducted as either VLOS or EVLOS operations (if the applicant holds an approval for EVLOS operations). Further approvals in addition to the BVLOS approval may then be required. If the applicant requests BVLOS operations with Class C or D airspace including military CTRs, Airservices Australia or the Defence unit controlling the airspace must be consulted (if the proposed operation is above 400 ft AGL, in the approach / departure path or within 3 NM of the movement area of the aerodrome). Such operations must be shielded at all times; radio transmissions and carriage are mandatory regardless of RPA size and the remote pilot must have the ability to monitor cooperative air traffic information (e.g. ADS-B IN receiver, web-based real time aircraft tracking services).| AU-STS | 

