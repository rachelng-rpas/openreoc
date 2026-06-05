# CASA Draft Annex A to AC 101-06 – Airworthiness-related OSOs (AusSORA)

**Author: Rachel Ng** | 6 June 2026

---

## Context and Status

> **This is not a regulatory change.** Draft Annex A to AC 101-06 is a CASA consultation — proposed advisory circular content open for industry feedback. The AAUS submission (5 May 2026) is industry's formal response. No rule has changed yet.

This draft sits within the broader **AusSORA framework** under AC 101-06, which adapts JARUS SORA 2.5 to Australian conditions. Annex A specifically addresses the **airworthiness-related Operational Safety Objectives (OSOs)** that operators must comply with as part of the AusSORA approval process.

**References:**
- [CASA AusSORA assessment requirements](https://www.casa.gov.au/aussora-assessment-requirements-and-criteria)
- [Draft Annex A – AC 101-06 v1.0 PDF](https://consultation.casa.gov.au/regulatory-program/draft-annex-a-to-ac-101-06/supporting_documents/draft-annex-a-to-ac-101-06-v10pdf)

---

## Who This Applies To

This document is primarily relevant to:

- **RPAS operators** applying for AusSORA approvals (especially SAIL III and above), who must demonstrate compliance with airworthiness-related OSOs as part of their application
- **RPAS OEMs and system designers** who need to provide design assurance data and evidence to support operator applications — the OSOs place obligations on the technical integrity of the system itself
- **Operators using COTS (commercial off-the-shelf) platforms**, who face the practical challenge of meeting OSO evidence requirements without full access to manufacturer design assurance data

Less directly applicable to lower-risk operations (SAIL I–II), though the framework still sets the conceptual baseline.

---

## What Is Being Proposed

### Background: OSOs and SAIL

Under AusSORA, each operation is assigned a **SAIL level (I–VI)**. For each SAIL, the operator must meet specific **Operational Safety Objectives (OSOs)** — safety goals that manage risk if the drone loses control.

Each OSO is assessed against a required **level of robustness**, which combines:
- **Level of integrity** — how well designed the safety objective is
- **Level of assurance** — how confidently it can be demonstrated

| SAIL | I | II | III | IV | V | VI |
|---|---|---|---|---|---|---|
| Robustness (example: OSO #04) | O | O | O | L | M | H |

*O = optional, L = low, M = medium, H = high*

### The Three OSOs in Annex A

Annex A currently covers three airworthiness-related OSOs:

**OSO #04 – UAS components essential to safe operations are designed to an airworthiness design standard (ADS)**
The UA's critical components must be designed to a recognised airworthiness standard appropriate to the SAIL level. Evidence requirements escalate from low (basic documentation) through to high robustness (formal design assurance aligned to standards like DO-178C, ARP4761).

**OSO #05 – RPAS is designed considering system safety and reliability**
The overall system — not just individual components — must demonstrate that system-level safety and reliability have been considered in the design. Includes failure mode analysis, reliability data, and safety case documentation scaled to the SAIL level.

**OSO #24 – UAS designed and qualified for adverse environmental conditions**
The UA must be designed and qualified to operate safely within the environmental envelope of the intended operation (temperature, wind, precipitation, etc.). Evidence must show the operating envelope is defined, tested, and not exceeded in the operational context.

### How Each OSO Is Structured in the Document

For each OSO, Annex A sets out:
1. Required level of robustness per SAIL level
2. Criteria to achieve each level of integrity
3. Criteria to achieve each level of assurance
4. Means of compliance — what evidence to provide and how CASA will assess it
5. Additional guidance, examples, and technical tips

---

## How to Read a Regulatory Consultation

Key mindset principles when reviewing a technical advisory circular like this:

| Principle | What it means in practice |
|---|---|
| **Conceptual foundation vs practical tool** | Ask: is this document usable as written, or does it still need supporting templates, examples, and tools before operators can actually apply it? A well-structured framework is not the same as a workable process. |
| **Evidence gap test** | For each requirement, ask: what exactly does CASA want to see, at what level of detail, and how should it be presented? If the document doesn't answer this clearly, there's a gap between the rule and the application. |
| **COTS reality check** | Most commercial operators don't have access to their aircraft's full design assurance data. Any OSO framework must accommodate hybrid compliance models — not just assume full OEM design data is available. |
| **Proportionality across SAIL** | Lower SAIL operations should not face the same documentation burden as higher-assurance operations. Check whether the framework clearly differentiates, or whether higher-assurance approaches are bleeding into lower-risk contexts. |
| **Outcome vs process** | Requirements should focus on safety outcomes, not documentation processes. If compliance is demonstrated by generating paperwork rather than reducing risk, the framework is misaligned. |
| **International alignment** | Where Australia diverges from EASA or FAA standards (e.g. FDAL thresholds), operators need to understand the implications for international operations and product recognition. |
| **Terminology consistency** | Technical frameworks depend on precise language. Where terms like TLOS and LOCO are used interchangeably or inconsistently with SORA 2.5, it creates ambiguity that flows through into every application. |

---

## AAUS Industry Themes – Summary

Recurring ideas from the AAUS submission, reflecting how experienced industry stakeholders think about a technical regulatory consultation.

| Theme | Core concern | Relevant section |
|---|---|---|
| **Evidence gap** | Annex A describes what robustness is required but not clearly enough what evidence demonstrates it, how it should be presented, or what CASA will accept. | Sections 4.1, 5.1, 5.2 |
| **COTS operator reality** | Many operators use commercial platforms without access to full OEM design assurance data. The framework must support hybrid and operationally-driven compliance models, not only full design assurance. | Sections 4.2, 5.3 |
| **Outcome-based, not process-driven** | Risk of over-reliance on documentation over genuine safety outcomes. Equivalent means of compliance and operational mitigations should be recognised as valid. | Section 4.3 |
| **SAIL proportionality** | Without clear differentiation between lower and higher SAIL expectations, lower-risk operators may face disproportionate burden — effectively applying certified-category standards to specific-category operations. | Section 4.4 |
| **Needs supporting tools to work** | Annex A is a conceptual foundation, not a standalone usable document. Worked examples, templates, and application guidance are required before it can support efficient approvals. | Sections 4.5, 5.2 |
| **Terminology and consistency** | TLOS vs LOCO usage is inconsistent with SORA 2.5. Tables 3 and 4 partially duplicate and create inconsistency in integrity vs assurance criteria. Specific terms like "minimise" and "probable" are undefined. | Section 5.1 |
| **Failure probability derivation** | Table 11 failure probability objectives may be an order of magnitude less conservative than required by SORA TLOS, because the derivation does not account for the proportion of LOCO attributable to technical failures. | Section 5.1 |
| **International alignment risk** | Where AusSORA FDAL thresholds diverge from EASA MoC without explanation, it creates barriers to international product recognition and export. Alignment supports adoption by overseas regulators and customers. | Section 5.1 |
| **Co-design with OEMs** | Effective implementation requires ongoing collaboration with manufacturers who understand design constraints — the framework should reflect how RPAS are actually designed and certified, not assume a manned-aviation model. | Section 4.2 |
