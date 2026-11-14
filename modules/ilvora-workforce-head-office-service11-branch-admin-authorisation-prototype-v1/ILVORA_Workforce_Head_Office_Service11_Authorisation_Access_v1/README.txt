ILVORA WORKFORCE
Head Office Admin Panel – Service 11: Branch Admin / HR Authorisation & Access Control
Prototype v1

RUN
1. Extract the ZIP.
2. Open index.html in Chrome or Edge.
3. Authorise one of the illustrative active employees, select a branch and permissions.
4. Explore the Access Register, Password Reset Desk, Employment Status Changes and Audit History.
5. Export the access register CSV or print/Save PDF.

INCLUDED
- Select existing employee by permanent Employee ID.
- Authorise Branch Admin / HR dashboard access for a selected branch.
- Select role and granular permissions.
- Simulate automatic temporary password generation and delivery to registered contact.
- First-login password-reset state.
- Head Office password reset desk with review / hold / reject outcomes.
- Simulated temporary password reset and forced-reset state.
- Revoke access on approved termination, resignation, ineligible position change or authorisation withdrawal.
- Branch transfer updates branch scope in demo.
- Access register, audit history, CSV export and print.

DEMO CREDENTIAL WARNING
The temporary passwords shown in this prototype are randomly generated demo strings for illustrating the workflow only. They are not sent by SMS/email, are not valid credentials, and must never be used for real accounts. Production must never display plaintext temporary passwords to administrators.

PRODUCTION REQUIREMENTS
- Use the existing Employee ID as username; do not create duplicate employee identities.
- Enforce server-side RBAC and branch-scoped permissions.
- Generate cryptographically secure, one-time temporary credentials with short expiry.
- Deliver only to verified registered contact channels using secure messaging providers.
- Store passwords using a modern password hash (e.g. Argon2id or appropriately configured bcrypt); never store or log plaintext.
- Force password change on first login and after reset.
- Apply rate limits, account lockout protections, secure session management and invalidate active sessions/tokens on revocation.
- Verify identity and active authorisation before password reset.
- Trigger access revocation from approved HR employment/position/branch changes using effective dates.
- Retain the employee master account and historical records; revoke only the relevant dashboard role/permissions.
- Maintain immutable audit logs without passwords, OTPs or secrets.
- Notify the employee and appropriate Head Office custodian when access is granted, changed or revoked.
- Apply legal/privacy review to contact details and access logs.

LIMITATIONS
Front-end demo only. Data resets on refresh. No live authentication, password delivery, OTP/SMS/email, database, Cloudflare integration, real role enforcement, HRIS event trigger or session revocation is connected.
Do not enter real employee personal data.
