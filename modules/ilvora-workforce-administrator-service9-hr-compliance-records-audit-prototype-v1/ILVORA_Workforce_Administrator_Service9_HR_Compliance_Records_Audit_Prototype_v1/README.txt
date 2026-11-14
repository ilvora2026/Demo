ILVORA Workforce – Administrator Service 9
HR Compliance, Records Retention & Audit Management – Prototype v1

Open index.html in a modern browser.

Includes:
- Central retention/compliance register
- Record reference, branch, category, review date and custodian
- Hold management (legal, audit, investigation and regulatory)
- Print and physical filing register
- Destruction review/audit history
- Retention policy reference table
- Filters and summary indicators

Important design rules reflected:
- Attendance detailed report: print by 15th of following month; eligible for digital deletion after 21st of following month, subject to hold and filing checks.
- Attendance summary: retain 3 years.
- Detailed duty roster: eligible for digital deletion after 15th of following month; brief summary retained 3 years.
- Medical certificates and legally required leave evidence: retain digitally 5 years, subject to legal review.
- Attendance photos: delete after 2 days under agreed design rule.
- Other employee, payroll, contract and statutory records: no generic deletion period; configure only under an approved HR/legal retention schedule.
- Legal, audit, investigation and regulatory holds pause deletion/destruction.
- Printing does not itself authorise digital deletion.
- Physical records require separate retention, access and secure destruction controls.

Prototype limitations:
- Fictional demo data only.
- No real authentication, role enforcement, database persistence, scheduled deletion, secure file storage, immutable audit log, or actual destruction.
- Changes are in-memory and reset on refresh.
- Demo date indicators are illustrative.

Production requirements:
- Approve an India/Kerala-specific legal retention schedule before configuring expiry.
- Enforce holds server-side and block all digital/physical destruction while a hold is active.
- Require authorised approval and evidence before destruction; retain destruction certificates.
- Separate digital and physical retention schedules.
- Use least-privilege access, encryption, immutable audit logs, backups and secure disposal.
- Maintain print/filing register with printed by, date, record reference, page count and physical storage location.
