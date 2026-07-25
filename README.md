# Northbridge Financial plc — Cyber & Information Resilience Policy

| | |
|---|---|
| **Document Owner** | Chief Information Security Officer (CISO) |
| **Approved By** | Board Risk Committee |
| **Classification** | Internal |
| **Version** | 1.0 |
| **Review Cycle** | Annual, or on material change |
| **Applies To** | All employees, contractors, and third parties with access to Northbridge systems, data, or connected devices |

---

## 1. Purpose

This policy sets out Northbridge Financial plc's mandatory requirements for protecting the confidentiality, integrity, and availability of its information assets, systems, and connected devices (including Operational Technology and IoT where applicable across the estate). It establishes the principles that all Standards, Procedures, and Guidelines within the Cyber & Information Resilience Framework must support.

## 2. Scope

This policy applies to all Northbridge-owned or Northbridge-managed technology, all data processed on behalf of Northbridge, and all personnel and third parties with access to either. It covers, without limitation: corporate IT systems, customer-facing platforms, physical security and building management systems, and any Internet of Things (IoT) or Industrial IoT devices connected to Northbridge networks.

## 3. Policy Statement

Northbridge Financial plc is committed to managing cyber risk in line with its Board-approved risk appetite, applicable regulatory obligations (including FCA requirements, UK GDPR, and the NIS Regulations where relevant), and recognised industry standards including ISO/IEC 27001, the NIST Cybersecurity Framework, and the NCSC Cyber Assessment Framework.

## 4. Core Requirements

| # | Requirement | Rationale |
|---|---|---|
| 4.1 | All systems and devices must be recorded in a maintained asset inventory before being connected to any Northbridge network. | An unrecorded device cannot be risk-assessed, patched, or monitored — see Project 1 finding R1/R7. |
| 4.2 | Default credentials must be changed and Multi-Factor Authentication enforced on all systems supporting it, before go-live. | Default/weak credentials were the root cause of the two highest-severity risks identified in the Northbridge IIoT audit (Case Study 1). |
| 4.3 | All systems must be maintained on vendor-supported software/firmware versions, with critical patches applied within Board-approved timeframes. | Directly addresses outdated-software risk (R6) and centralised platform compromise (R7). |
| 4.4 | Network segmentation must separate IoT/OT devices from core IT and safety-critical infrastructure. | Prevents lateral movement from a compromised low-trust device to high-value systems. |
| 4.5 | Any deviation from a mandatory Standard requires an approved Policy Waiver before implementation — see Section 6. | Ensures risk is knowingly accepted at the appropriate level, not silently absorbed. |
| 4.6 | All colleagues with system access must complete annual cyber awareness training. | Addresses human-layer risk not covered by technical controls. |

## 5. Roles and Responsibilities

| Role | Responsibility |
|---|---|
| **Board Risk Committee** | Approves this policy and the organisation's cyber risk appetite; receives quarterly reporting on residual risk. |
| **CISO** | Owns the policy framework; approves Standards; escalates material non-compliance. |
| **Cyber Policy Lead** | Maintains and refreshes the policy suite; manages the Waiver process; conducts gap analysis and horizon scanning. |
| **System/Risk Owners** | Ensure systems under their control comply with this policy and supporting Standards; hold and track any approved Waivers. |
| **All Colleagues** | Complete required training; report suspected non-compliance or incidents without delay. |

## 6. Exceptions and Waivers

Where a system or business need cannot meet a mandatory requirement, a Policy Waiver must be raised, risk-assessed, time-bound, and approved at a level proportionate to the residual risk (see the [Policy Waiver Process](./policy-waiver-process.md)). Waivers do not remove a requirement — they record a knowingly accepted, time-limited exception.

## 7. Non-Compliance

Non-compliance identified outside an approved Waiver will be logged, risk-assessed, and reported through the governance channels described in Section 8. Persistent or high-risk non-compliance will be escalated to the relevant Director.

## 8. Governance and Reporting

This policy is supported by a framework of Standards, Procedures, and Guidelines. Compliance status, open Waivers, and gap-analysis findings are reported monthly to the CISO and quarterly to the Board Risk Committee.

---

## Supporting Documents in This Repository

- [Standard on a Page — Access Control](./standard-on-a-page-access-control.md) — a simplified, single-page format for one mandatory Standard, demonstrating the "standards on a page" approach to improving usability and adoption
- [Policy Waiver Process](./policy-waiver-process.md) — the request form, approval thresholds, and register used to manage exceptions to this Policy
- [Gap Analysis — NIST CSF 2.0](./gap-analysis-nist-csf-2.md) — a horizon-scanning exercise assessing this framework against the current version of NIST CSF, identifying required updates

*This is a fictional case study built for portfolio purposes, developed as a companion piece to the IIoT Airport Risk Assessment repository — that project surfaces the kind of findings (weak credentials, unpatched centralised platforms) this framework is designed to catch before they happen.*
