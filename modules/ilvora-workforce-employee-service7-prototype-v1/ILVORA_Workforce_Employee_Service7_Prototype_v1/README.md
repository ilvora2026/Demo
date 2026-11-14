# ILVORA Workforce – Employee Service 7 Prototype v1
## My Notifications & Announcements

### Included
- Personal notification centre with unread count.
- Filters for attendance, leave, payroll, duty roster, announcements, unread and action-required items.
- Search, view details, mark individual notifications read and mark all read.
- Scope labels for personal, branch and organisation-wide notices.
- Sample alerts for attendance corrections, leave decisions, payslip requests, rosters and company policies.

### Demo limitations
This is a front-end demonstration with sample data. It does not connect to authentication, a database, push notifications, email, SMS, payroll, attendance or HR workflows. Read/unread state is held in browser memory and resets on refresh.

### Production requirements
- Generate notifications from verified server-side events and enforce employee/branch role permissions.
- Keep a durable notification record with recipient, source event, category, scope, timestamps and read status.
- Deliver in-app notifications; use approved email/SMS/push channels only where configured and consented/legally permitted.
- Avoid exposing sensitive medical, payroll or personal information in lock-screen previews or email subject lines.
- Provide delivery/retry logs, user notification preferences, retention rules and audit history.
- Announcement publication must be permission-controlled; retain the published version and effective dates.
- Link actions to the relevant secure service and re-check permissions server-side.
