# Gap Analysis: Northbridge Cyber Policy Framework vs NIST CSF 2.0

*Companion to the [Cyber & Information Resilience Policy](./README.md) — demonstrating the horizon-scanning and gap-analysis activity described in the framework's governance model*

---

## 1. Why this analysis

NIST released Cybersecurity Framework (CSF) 2.0 in February 2024 — the first major revision since the original 2014 framework. Northbridge's policy framework in this repository was built with NIST CSF's five original functions in mind (Identify, Protect, Detect, Respond, Recover). This is a worked example of the kind of horizon-scanning exercise a Cyber Policy Lead would run whenever a referenced standard changes: does the current framework still meet the standard it claims to follow, and what needs updating.

## 2. What actually changed in CSF 2.0

The headline change is the addition of a sixth function, **Govern**, sitting alongside the original five. NIST CSF 2.0 elevates governance — organisational context, risk management strategy, roles and responsibilities, policy, and oversight — to a first-class function in its own right, rather than treating it as background context for the other five. The framework was also broadened beyond its original critical-infrastructure focus to explicitly apply to organisations of any size or sector.

## 3. Gap Analysis Table

| CSF 2.0 Function | Current Framework Coverage | Gap Identified | Recommended Update |
|---|---|---|---|
| **Govern** *(new in 2.0)* | Partial — Section 8 of the Policy covers reporting and Section 5 covers roles, but there is no single place addressing organisational risk strategy, supply chain risk governance, or how cyber risk appetite is set and communicated. | The Policy currently treats governance as scattered context rather than a defined, ownable function. This is the highest-priority gap, since Govern is the newest and most emphasised addition in 2.0. | Add a dedicated **Governance Standard** setting out: how risk appetite is set and reviewed (linking to the Board Risk Committee), how supply chain/third-party cyber risk is assessed before onboarding, and how policy itself is governed (versioning, review cycle, approval chain) — much of which already exists informally across this framework but isn't yet consolidated under one Standard. |
| **Identify** | Strong — Section 4.1 (asset inventory) and the risk register model from the linked case study cover this well. | Minor — no explicit reference to supply chain risk identification for third-party/vendor-managed IoT devices (relevant given the Axis and Honeywell findings in the linked case study). | Extend the Asset Inventory requirement to explicitly capture vendor/third-party ownership and support status per device. |
| **Protect** | Strong — Section 4.2–4.4 (access control, patching, segmentation) map directly onto Protect. | None significant. | No action required. |
| **Detect** | Weak — the Policy references monitoring in passing (Recommendation 1 in the linked case study) but has no Standard defining detection requirements, log retention, or anomaly-detection scope. | This is the second-largest gap — CSF 2.0 expects clear detection capability, and the current framework only implies it exists. | Add a **Security Monitoring Standard** defining minimum logging, retention periods, and anomaly-detection coverage across IoT/OT estates. |
| **Respond** | Not currently addressed in this framework. | No incident response process exists in the documents in this repository. | Out of scope for this portfolio extract, but flagged as the next Standard to develop — a real framework would not be complete without it. |
| **Recover** | Not currently addressed in this framework. | Same as above. | Same as above — flagged for future work, not fabricated here for the sake of appearing complete. |

## 4. Prioritised Recommendations

1. **Immediate:** Draft the Governance Standard — this is both the newest requirement in CSF 2.0 and the one with the clearest existing foundation to build from (Sections 5 and 8 of the current Policy).
2. **Next cycle:** Draft the Security Monitoring Standard, closing the Detect gap.
3. **Flagged, not actioned in this extract:** Respond and Recover Standards are genuine gaps in a real framework, and are intentionally left open here rather than padded out — a live gap analysis should be honest about what hasn't been built yet, not just what has.

## 5. Why this matters for a Policy Lead role

This is the core of ongoing framework maintenance: standards don't stay current on their own, and a "review annually" clause in a policy document is only useful if someone actually runs the comparison when the underlying standard changes. This table is a concrete, evidenced example of that comparison — including being explicit about what's genuinely unfinished, rather than overstating coverage to make the framework look more complete than it is.

---

*Reference: National Institute of Standards and Technology (2024)* The NIST Cybersecurity Framework (CSF) 2.0*. NIST CSWP 29. Available at: https://www.nist.gov/cyberframework (Accessed: 25 July 2026)*

*Related documents: [Cyber & Information Resilience Policy](./README.md) · [Policy Waiver Process](./policy-waiver-process.md)*
