ILVORA Workforce – Administrator Service 12
Finance & Operational Expense Management – Prototype v1

Open index.html in a modern browser.

Confirmed authority:
- The Managing Director sets and may revise the Administrator's expense approval limit.
- Expenses at or below the currently MD-approved limit may be approved by the Administrator.
- Expenses above the limit require Managing Director approval.
- Until a numerical limit is formally configured and approved by the MD, all expenses are routed to the MD.
- Branch Admin/HR submit expenses and supporting documents; they do not approve expenses.

Features:
- Branch-wise expense register and categories
- Expense submission with bill/invoice reference and attachment filename field
- Recurring expense and due-date fields
- Approval routing based on MD-configured limit
- MD limit configuration demonstration
- Expense review status and audit history
- Budget/payment governance guidance
- CSV export and print / Save as PDF

Prototype limitations:
- Fictional sample data only.
- No real authentication, role enforcement, backend/database persistence, invoice file storage, accounting integration, payment processing, tax computation or bank verification.
- Changes are in-memory and reset on refresh.
- The MD limit control is not protected by real authentication; it is a demonstration only.

Production requirements:
- Implement MD-only limit configuration and approval server-side.
- Maintain effective-dated limit history and approval evidence.
- Enforce no self-approval and separation of duties.
- Verify invoices, detect duplicates, retain payment proofs and record transaction references.
- Integrate approved budgets, liabilities and payments with accounting/payroll as appropriate.
- Use secure evidence storage, role-based access, immutable audit logs and physical filing controls.
- Obtain accounting/tax/legal review for expense categories, approvals and statutory records.
