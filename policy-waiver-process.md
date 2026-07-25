# Policy Waiver Process

*Companion to the [Cyber & Information Resilience Policy](./README.md) — Section 6*

---

## 1. Why this process exists

Not every system can meet every Standard on day one — legacy platforms, vendor constraints, or delivery timelines sometimes make full compliance impractical in the short term. The Waiver process exists so that gap is **knowingly accepted at the right level, time-bound, and tracked to closure** — rather than silently absorbed and forgotten, which is how governance gaps like the ones identified in the Northbridge IIoT audit (Project 1) go undetected for a decade.

A Waiver is not a way around a Standard. It's a record that says: *we know we don't meet this requirement, here's why, here's what we're doing to reduce the risk in the meantime, and here's when it stops being acceptable.*

## 2. When a Waiver is required

A Waiver must be raised **before** a system goes live, or **immediately** on discovering existing non-compliance, whenever a system or process cannot meet a mandatory requirement in the Cyber & Information Resilience Policy or its supporting Standards. Examples from the Northbridge context:

- A legacy building management system that cannot support MFA (a real constraint identified in the Honeywell XL Web II evaluation in Project 1)
- A vendor-managed device where firmware updates are outside Northbridge's direct control
- A time-limited pilot deployment where full network segmentation isn't yet built

## 3. Process Flow

```
1. REQUEST
   Risk/System Owner completes the Waiver Request Form (Section 5)
   ↓
2. RISK ASSESSMENT
   Risk team scores likelihood/impact using the standard risk matrix
   Compensating controls are reviewed for adequacy
   ↓
3. APPROVAL (proportionate to residual risk)
   Low residual risk    → Risk Lead approval
   Medium residual risk  → CISO approval
   High/Critical residual risk → Board Risk Committee approval
   ↓
4. REGISTRATION
   Approved Waiver is logged in the Waiver Register with an expiry date
   ↓
5. MONITORING
   Waiver status reviewed monthly; owner reminded ahead of expiry
   ↓
6. CLOSURE OR RENEWAL
   Either the underlying gap is fixed and the Waiver is closed,
   or a renewal is requested with updated justification —
   Waivers do not renew automatically
```

## 4. Approval Thresholds

| Residual Risk (post compensating controls) | Approver | Max Duration |
|---|---|---|
| Low | Risk Lead | 12 months |
| Medium | CISO | 6 months |
| High | CISO + notify Board Risk Committee | 3 months |
| Critical | Board Risk Committee | 1 month, with an active remediation plan required |

No Waiver may be approved as permanent. Every Waiver carries an expiry date; a Waiver with no planned remediation path should be treated as a proposal to formally accept the risk (a separate governance decision), not a Waiver.

## 5. Waiver Request Form (Template)

| Field | Detail |
|---|---|
| **Waiver ID** | *(auto-assigned, e.g. WAV-2026-014)* |
| **Requested By** | *(name, role)* |
| **System/Process Affected** | *(e.g. Honeywell XL Web II — Terminal 3 BMS)* |
| **Requirement Not Met** | *(cite the specific Policy/Standard clause, e.g. "Access Control Standard 4.2 — MFA required")* |
| **Reason Compliance Isn't Currently Possible** | *(technical, contractual, or timeline constraint — be specific)* |
| **Compensating Controls in Place** | *(what's mitigating the gap in the meantime — e.g. network segmentation, enhanced monitoring, restricted physical access)* |
| **Residual Risk Rating** | *(Low / Medium / High / Critical — per standard risk matrix)* |
| **Requested Duration** | *(start date → expiry date)* |
| **Remediation Plan** | *(what will actually close this gap, and by when — a Waiver without a remediation plan should be escalated as risk acceptance instead)* |
| **Approver** | *(per Section 4 thresholds)* |
| **Approval Date** | |
| **Review/Expiry Date** | |

## 6. Waiver Register (tracking)

All approved Waivers are logged centrally so status is visible without chasing individual owners:

| Waiver ID | System | Requirement Waived | Residual Risk | Approver | Expiry | Status |
|---|---|---|---|---|---|---|
| WAV-2026-014 | Honeywell XL Web II (T3 BMS) | MFA (Access Control 4.2) | Medium | CISO | 2026-10-01 | Open |
| WAV-2026-015 | Axis Camera Station legacy build | Patch to v5.58 (Standard 4.3) | High | CISO + Board notified | 2026-08-15 | Open |

## 7. Reporting

Open Waivers, upcoming expiries, and any Waiver approaching its second renewal (a signal the underlying problem isn't actually being fixed) are reported monthly to the CISO and summarised quarterly to the Board Risk Committee alongside the wider risk register — closing the loop back to the governance model described in the [Cyber & Information Resilience Policy](./README.md).

---

*Related documents: [Cyber & Information Resilience Policy](./README.md) · [Standard on a Page — Access Control](./standard-on-a-page-access-control.md)*
