ILVORA Workforce – Administrator Service 4
Employee Account Access & Deactivation Prototype v1

RUN
1. Extract the ZIP.
2. Open index.html in a modern browser.
3. Explore the employee account register, request queue, access action, audit history,
   and rules/permissions tabs.

INCLUDED
- Sample employee account directory with branch filtering.
- Account and employment status overview.
- Resignation and termination access request queue.
- Demo actions for suspension, reactivation, deactivation and scheduled resignation end.
- Effective date, last working day, reference and reason capture.
- Access-change audit history concept.
- Role permission boundaries and production safeguards.

LIMITATIONS
- Front-end demonstration only; all records are fictional.
- No authentication, backend, database, actual account deactivation, session revocation,
  approval verification, scheduled job, notification or live audit service.
- Demo changes are in browser memory and reset on refresh.
- Do not enter real employee or personal information.

GOVERNANCE
- Branch Admin / HR may submit requests but cannot deactivate employee accounts.
- Administrator performs authorised account access actions after verifying approval.
- Resignation access ends at the end of the approved last working day.
- Termination access ends at the approved effective date/time.
- Deactivation must not delete employee records, attendance, payroll, leave, payslips,
  signed contracts or statutory documents.
- Production requires server-side RBAC, MFA for privileged accounts, revocation of active
  sessions/tokens, immutable audit logging, effective-dated processing and retention controls.
