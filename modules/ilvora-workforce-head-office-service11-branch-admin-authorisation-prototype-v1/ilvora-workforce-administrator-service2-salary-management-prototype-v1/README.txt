ILVORA Workforce – Administrator Service 2
Employee Salary Management Prototype v1

HOW TO RUN
1. Extract the ZIP.
2. Open index.html in a modern browser (Chrome, Edge or Firefox).
3. Use the tabs to inspect the salary register, add/revise salary, revision history and governance.

INCLUDED
- Employee salary register with ID/name and branch filters.
- Add/revise fixed monthly salary with effective date and reason.
- Monthly allowances and deductions with a simple net-pay preview.
- Pending-change/revision history concept.
- Role permission boundaries and production governance checklist.
- Print current view.

IMPORTANT LIMITATIONS
- Front-end demonstration only. Sample employee records are fictional.
- No real login, access enforcement, database, API, payroll processing, approval service,
  statutory deduction engine, payslip generation, email/SMS, or audit backend.
- Demo data exists only in the page's JavaScript memory and resets on refresh.
- Do not enter real employee, bank, Aadhaar, PAN or salary information.

GOVERNANCE DESIGN
- Administrator can enter and revise salary records.
- Branch Admin/HR and Head Office Admin cannot change salary amounts.
- Salary changes are represented as pending until an independent approval workflow is
  implemented. The requester must not approve their own change.
- Approved, effective-dated salary versions should be retained as history and only approved
  versions should flow into payroll.
- Production requires legal/payroll review of statutory deductions and secure server-side
  role-based access, encryption, audit logs and data retention controls.
