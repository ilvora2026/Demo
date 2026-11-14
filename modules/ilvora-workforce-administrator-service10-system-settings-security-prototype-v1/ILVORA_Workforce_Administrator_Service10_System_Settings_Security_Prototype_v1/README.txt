ILVORA Workforce – Administrator Service 10
System Settings & Security Management – Prototype v1

Open index.html in a modern browser.

Includes:
- Password and login policy configuration
- OTP and account recovery policy
- Session register and demo force-logout controls
- Security notification preferences
- Backup and recovery policy settings
- Role and permission governance overview
- Security event and configuration audit register
- Demo CSV audit export

Governance boundaries:
- Administrator manages operational system settings and security configuration.
- Head Office Admin controls branch setup, employee approval and Branch Admin/HR authorisations.
- Branch Admin/HR operates within assigned branch and delegated permissions.
- Managing Director retains executive oversight and reserved approval authority.
- Employee access is limited to own employee self-service records.

Prototype limitations:
- Front-end demonstration only; no real authentication, server-side RBAC, MFA, OTP delivery, session revocation, database persistence, backups, notifications or production security changes.
- Demo settings and session actions are not enforced.
- Data resets on refresh; all events and users are fictional.

Production requirements:
- Enforce all settings server-side; never rely on browser-only controls.
- Use secure password hashing (Argon2id or appropriately configured bcrypt), MFA for privileged roles, breached-password screening, rate limits and secure account recovery.
- Store session tokens securely; revoke sessions and refresh tokens server-side.
- Deliver OTP only through verified channels, with expiry, one-time use and attempt limits.
- Use least-privilege RBAC, branch-scoped access, immutable audit logs and alerts.
- Encrypt backups, store them separately, test restoration, and define RPO/RTO.
- Never log passwords, OTPs, access tokens or sensitive employee data.
