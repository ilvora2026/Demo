ILVORA Workforce — Managing Director Executive Command Centre
Version 1 — Consolidated front-end prototype

CONTENTS
- index.html: integrated MD dashboard prototype
- This README

RUN
1. Extract the ZIP.
2. Open index.html in Chrome, Edge or another modern browser.
3. Use the left navigation to open the Executive Overview, all 15 Administrator service visibility pages, all 10 additional MD executive services, and the 3 special executive features.

FINAL STRUCTURE INCLUDED
A. All 15 Administrator services, with organisation-wide MD visibility:
1 Dashboard; 2 Employee Salary Management; 3 Payroll Management; 4 Employee Account Access & Deactivation; 5 Payslip Authorisation; 6 Payroll Reports & Reconciliation; 7 Employee Advances & Loans; 8 Employee Compliance & Disciplinary; 9 Records Retention & Audit; 10 System Settings & Security; 11 System Monitoring & Technical Operations; 12 Finance & Operational Expense Management; 13 Procurement, Inventory & Asset Management; 14 Contracts & Agreement Management; 15 Licences, Registrations & Statutory Compliance.

B. Ten additional MD executive services:
16 Executive Intelligence Dashboard; 17 Strategic Planning & Business Development; 18 Investment & Capital Allocation; 19 Clinical Governance & Patient Safety; 20 Leadership & Management Performance; 21 Board, Shareholder & Investor Relations; 22 Enterprise Risk & Crisis Command; 23 Group Marketing & Brand Management; 24 Executive Decisions & Approval Centre; 25 Executive Confidential Vault.

C. Three special executive features:
- MD Daily Briefing
- Group Performance Scorecard
- Executive Decision Register

GOVERNANCE / AUTHORITY RULES REFLECTED
- MD has organisation-wide visibility across Head Office – Kochi, Neelambari Hospital – Thamarakulam and ILVORA Health Clinic – Kottarakkara.
- Administrator remains responsible for routine operational execution and delegated approvals.
- MD reserved authority includes final disciplinary decisions; employee advances above 25% of monthly salary; approval of expenses and procurement above MD-set delegated limits; setting/revising the Administrator's expense and procurement limits; and reserved / above-limit contract and strategic commitments.
- Until a numerical expense, procurement or contract approval limit is formally set and effective-dated, route the relevant commitment to MD.
- Head Office Admin Panel access credentials and authorisation are generated/issued by Administrator, following the same controlled access workflow as Branch Admin/HR.
- Confidential clinical, employee, grievance, legal and investigation information remains subject to need-to-know access, applicable law and independent conflict-of-interest safeguards.
- MD visibility does not automatically make MD the routine operator of every Administrator workflow.

IMPORTANT LIMITATIONS
This is a front-end navigation and workflow demonstration, not a live production application. It does not connect to Cloudflare D1, GitHub, real employee records, payroll, attendance, leave, procurement, contracts, regulatory portals, authentication, OTP/SMS/email, file storage, e-signature, payment systems or live notifications.
- All dashboard values, financial figures, branch KPIs, patient volumes, pending items, and examples are fictional illustrative data.
- Administrator service pages are executive visibility / governance summaries, not the previously approved standalone operational prototypes merged into a live system.
- Demo approval actions do not execute real approvals.
- Decision Register entries persist only for the current browser session; they are not stored in a backend.
- The Executive Confidential Vault is a design placeholder; no files are uploaded or stored.
- No live automatic daily briefing or scheduled notification runs.

PRODUCTION INTEGRATION REQUIRED
1. Integrate all approved Employee, Branch Admin/HR, Head Office Admin, Administrator and MD services into one authenticated application.
2. Use server-side RBAC and branch-scoped permissions; MD organisation-wide access must still respect statutory privacy, need-to-know, case conflicts and legal restrictions.
3. Connect Cloudflare Workers / D1 and private encrypted object storage; implement backups and restore tests.
4. Use immutable audit events for access, exports, approvals, changes and decisions.
5. Implement secure MFA/OTP, password hashing, session revocation, notification delivery logs and rate limits.
6. Implement approval-limit enforcement, effective dates, separation of duties and no self-approval.
7. Connect verified data sources for daily briefing and scorecards; show source, reporting period, freshness and missing-data indicators.
8. Use legal/HR/clinical governance review for sensitive data, retention, consent, and regulatory compliance.
9. Test role permissions, branch isolation, escalation, failure handling and disaster recovery before production deployment.

This ZIP is a consolidated MD design prototype. It does not imply that the production system has been deployed or that any real ILVORA data has been connected.
