# ILVORA Workforce – Branch Admin / HR Service 1 Prototype v1
## Branch Dashboard

### Included in this prototype
- Branch-scoped dashboard for Neelambari Hospital – Thamarakulam (demo).
- Workforce summary: active employees, present today, approved leave and attendance exceptions.
- Quick-action navigation placeholders for branch services.
- Action-required panel for leave reviews, attendance exceptions, policy acknowledgements and helpdesk requests.
- Daily attendance snapshot.
- Integrated Attendance Marker / Kiosk entry point.
- Responsive desktop and mobile layout using ILVORA navy, teal and champagne-gold branding.

### Role and permission principles
- Branch Admin / HR sees only the assigned branch by default.
- Head Office may grant broader scope through explicit permissions.
- Attendance Marker is a capability within the Branch Admin / HR module, not an automatic grant of all HR permissions.
- Attendance Operator can assist with kiosk check-in/check-out and monitor punches but cannot edit attendance, approve corrections, manage employees or access HR records unless separately authorised.
- Branch Admin / HR can review branch attendance and submit formal correction requests to Head Office; cannot approve its own correction request or directly alter verified attendance records.
- Complaints require case-level restricted access. A person named in a complaint must be bypassed from access and routing.

### Demo limitations
This is a front-end dashboard prototype with illustrative sample data. Navigation tiles open explanatory placeholders. There is no real login, database, attendance feed, employee directory, leave engine, notification service, permission enforcement or backend integration.

### Production requirements
- Enforce authentication, branch scoping and role permissions server-side.
- Calculate dashboard figures from authoritative records and display a data refresh timestamp.
- Log access to sensitive employee and complaint information.
- Use audited workflows for leave, attendance corrections, employee records and policy acknowledgements.
- Do not expose confidential complaint content in general branch dashboard widgets.
