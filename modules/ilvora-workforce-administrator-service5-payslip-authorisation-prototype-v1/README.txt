ILVORA Workforce – Administrator Service 5
Employee Payroll Requests & Payslip Authorisation Prototype v1

RUN
1. Extract the ZIP.
2. Open index.html in Chrome, Edge or Firefox.
3. Explore Request Queue, Review & Decision, Payslip Register, Audit History,
   and Security & Workflow.

FEATURES
- Employee payslip request queue with employee, branch, month and status filters.
- Verify payroll period is closed and locked before approval.
- Approve, reject or return requests with a required decision note.
- Block approval where payroll is not closed.
- Payslip register and reissue-request concept.
- Audit history for decisions and generation authorisations.
- Role permissions and secure delivery requirements.

LIMITATIONS
- Front-end demo only; all names, IDs and payroll records are fictional.
- No real PDF generation, secure storage, employee login, email/app notification,
  payroll connector, backend approval or access enforcement.
- Demo actions are local browser interactions and reset on refresh.
- Do not enter real employee, salary, bank, Aadhaar or PAN information.

PRODUCTION REQUIREMENTS
- Generate only from approved, locked payroll snapshots.
- Store payslips in private encrypted object storage.
- Require authenticated employee access and short-lived, expiring download URLs.
- Reissue as a new document version; retain previous audit history.
- Notify only the employee's verified registered contact/account.
- Log request, approval, generation, access and download events.
- Enforce server-side RBAC, rate limits, anti-enumeration and cross-employee isolation.
- Apply approved retention, legal hold and secure deletion schedules.
