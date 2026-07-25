# Standard on a Page: Access Control

*Companion to the [Cyber & Information Resilience Policy](./README.md) — Section 4.2*

---

**What this Standard is for:** Stopping unauthorised access to Northbridge systems and connected devices — the single largest driver of the risks identified in the Northbridge IIoT audit.

---

### ✅ You must

- Change every default password/credential before a device or system goes live
- Enable Multi-Factor Authentication (MFA) wherever the platform supports it
- Assign access on a least-privilege, role-based basis — not broad/shared accounts
- Review access rights for your systems at least every 6 months
- Remove access within 24 hours of a role change or leaver

### 🚫 You must not

- Use vendor default or shared credentials in production
- Store passwords in plaintext, in code, or in unencrypted config files
- Grant standing admin access where time-bound/just-in-time access is available

### ⚠️ If you can't meet this Standard

Raise a **Policy Waiver** before go-live — see the [Waiver Process](./policy-waiver-process.md). Do not proceed and plan to "fix it later."

### 🔍 How this gets checked

- New systems: reviewed at design/go-live gate by the Risk team
- Existing systems: sampled in the quarterly access review
- Non-compliance found outside a Waiver is logged and reported to the CISO monthly

### 🧭 Why it matters (in one line)

Two of the highest-severity risks in the Northbridge IIoT case study — unauthorised camera access and a pre-authentication compromise of the camera management platform — trace directly back to weak or default credentials. This is the cheapest control to get right and the most expensive to get wrong.

---

*Full technical requirements, exceptions criteria, and control mapping (ISO 27001 A.9, NIST CSF PR.AC): see the detailed Access Control Standard [not included in this portfolio extract].*
