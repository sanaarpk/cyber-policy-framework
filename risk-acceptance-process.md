# Risk Acceptance Process

*Companion to the [Cyber & Information Resilience Policy](./README.md) and the [Policy Waiver Process](./policy-waiver-process.md)*

---

## 1. Risk Acceptance vs a Waiver — why these are different instruments

A **Waiver** (see the [Policy Waiver Process](./policy-waiver-process.md)) is for gaps that are being actively fixed — it's time-bound, always carries a remediation plan, and expires. It's the right tool when the question is *"how long until this is compliant?"*

A **Risk Acceptance** is for gaps that will not be fixed in the foreseeable future — the cost, technical constraint, or business reality means full compliance isn't realistically achievable on any near-term timeline. It's the right tool when the honest answer to *"when will this be compliant?"* is *"not soon, and possibly not until the system is replaced."*

Conflating the two is a common governance failure: gaps get logged as Waivers, repeatedly renewed because the remediation plan was never real, and the organisation ends up carrying long-term risk with none of the senior visibility a genuine permanent gap deserves. The Northbridge Waiver Register template flags any Waiver approaching a second renewal specifically to catch this pattern and force a decision: fix it, or formally accept it.

| | Waiver | Risk Acceptance |
|---|---|---|
| **Use when** | Gap is being actively remediated | Gap has no realistic near-term fix |
| **Duration** | Time-bound, max 12 months, does not auto-renew | Reviewed annually, but can persist as long as the underlying constraint does |
| **Remediation plan** | Mandatory | Optional — often "replace the system" on a multi-year capital cycle |
| **Approval level** | Proportionate to residual risk (Risk Lead → Board, see Waiver Process) | Always Director-level minimum; Critical risk requires Board Risk Committee |
| **Renewal pattern** | Should not renew more than once without escalation | Reviewed, not renewed — a live decision each year, not a rubber stamp |

## 2. When to use Risk Acceptance

- The system is end-of-life or vendor-unsupported, and replacement is on a capital/budget cycle measured in years, not months
- A Waiver has been renewed once already with no meaningful progress on remediation (see Section 1) — this is the trigger to escalate rather than renew again
- The compensating controls in place are assessed as genuinely sufficient to hold the residual risk at an acceptable level indefinitely, not just temporarily

## 3. Risk Acceptance Form (Template)

| Field | Detail |
|---|---|
| **Risk Acceptance ID** | *(auto-assigned, e.g. RA-2026-003)* |
| **Requested By** | *(name, role)* |
| **System/Process Affected** | |
| **Requirement Not Met** | *(cite the specific Policy/Standard clause)* |
| **Why This Cannot Be Remediated in the Near Term** | *(be specific — vendor end-of-life, no patch path, capital cycle timing, etc. This is not a place for "we haven't gotten to it yet" — that belongs in a Waiver.)* |
| **Compensating Controls** | *(what is holding the residual risk at an acceptable level, and why those controls are assessed as sufficient long-term, not just adequate for now)* |
| **Residual Risk Rating** | *(Low / Medium / High / Critical)* |
| **Risk Owner** | *(the individual accountable for this risk remaining acceptable — not just who raised the form)* |
| **Business Justification** | *(why the cost/disruption of immediate remediation outweighs the residual risk being carried)* |
| **Approver** | *(Director minimum; Board Risk Committee for High/Critical)* |
| **Approval Date** | |
| **Next Review Date** | *(annual, non-negotiable — even permanent acceptances get re-examined)* |

## 4. Worked Example

To make this concrete rather than purely templated, here's a plausible completed example grounded in the linked case study — the Honeywell building management estate identified in the [IIoT Airport Risk Assessment](https://github.com/sanaarpk/iiot-airport-risk-assessment).

| Field | Detail |
|---|---|
| **Risk Acceptance ID** | RA-2026-003 |
| **Requested By** | Head of Facilities |
| **System/Process Affected** | Honeywell XL Web II controllers — Terminals 1–3 (12 units) |
| **Requirement Not Met** | Access Control Standard 4.2 — MFA required on all systems supporting it |
| **Why This Cannot Be Remediated in the Near Term** | The XL Web II platform does not support MFA at a protocol level — this is a vendor architectural limitation, not a configuration gap. Honeywell has confirmed end-of-life status for this product line, with no MFA support planned. Full replacement is scoped into the Terminal Systems Capital Programme, currently budgeted for FY2028. |
| **Compensating Controls** | Network segmentation isolating BMS controllers on a dedicated VLAN with no internet-facing access; access restricted to a named list of 4 facilities engineers via jump-host with its own MFA; all BMS network traffic logged and reviewed monthly; physical access to controller cabinets restricted and alarmed. |
| **Residual Risk Rating** | Medium (down from High pre-controls) |
| **Risk Owner** | Head of Facilities, with quarterly attestation to the CISO that compensating controls remain in place |
| **Business Justification** | Early replacement (outside the planned FY2028 programme) would cost an estimated £180k in accelerated capital spend and require terminal-area works disruption, against a residual risk already reduced to Medium by compensating controls. The FY2028 timeline is accepted as reasonable given the controls in place. |
| **Approver** | CISO, with Board Risk Committee notified given the Critical-infrastructure context (per Section 5) |
| **Approval Date** | 2026-07-01 |
| **Next Review Date** | 2027-07-01 |

## 5. Approval and Escalation

| Residual Risk | Minimum Approver | Board Visibility |
|---|---|---|
| Low | Director | Logged in quarterly risk report |
| Medium | CISO | Notified in quarterly risk report |
| High | CISO + Board Risk Committee notification | Named individually in quarterly report |
| Critical | Board Risk Committee approval required | Standing agenda item until reviewed or resolved |

## 6. Register and Ongoing Governance

All accepted risks are logged in a Risk Acceptance Register, reported alongside the Waiver Register described in the [Policy Waiver Process](./policy-waiver-process.md), so the CISO and Board see the complete picture of both temporary exceptions and permanent accepted risk in one place — not two disconnected lists that make total exposure hard to see.

| RA ID | System | Requirement Waived | Residual Risk | Next Review |
|---|---|---|---|---|
| RA-2026-003 | Honeywell XL Web II (T1–T3 BMS) | MFA (Access Control 4.2) | Medium | 2027-07-01 |

---

*Related documents: [Cyber & Information Resilience Policy](./README.md) · [Policy Waiver Process](./policy-waiver-process.md) · [Gap Analysis — NIST CSF 2.0](./gap-analysis-nist-csf-2.md)*
