ILVORA WORKFORCE – RESIGNATION & EXIT WORKFLOW PROTOTYPE v2

New rules added:
1. All company access is automatically disabled on the next calendar day after the approved last working day.
   Production access closure scope should include employee portal, company email, internal apps, SSO sessions, VPN/remote access and physical access credentials where integrated.
   Example: approved last working day 30 November -> access disabled 1 December at 00:00 local time.
2. Employee certificate request window opens 5 calendar days before the approved last working day.
3. Employee receives an automated reminder 7 calendar days before the approved last working day to apply for certificates.
4. Certificate is generated/issued only after the approved last working day has passed and all company exit clearances are complete.
5. Every resignation requires final MD approval.
6. Preserve employee, attendance, payroll, leave, contract, certificate and statutory records after access deactivation.

Prototype tabs:
- Employee Portal
- Branch Admin / HR
- Head Office Admin
- Administrator
- Managing Director
- Exit Automation Register

IMPORTANT:
This is a front-end prototype. Notifications, scheduler, access deactivation, role authentication, workflow routing and database operations are illustrative only. No real accounts, email, SMS, SSO, VPN or physical access control are connected. Production requires server-side scheduled jobs, reliable retries, timezone-aware event handling, audit logging, access-provider integrations, notification delivery records and exception handling.

Certificate window uses calendar days. The employee may request within the five-calendar-day period before the approved last working day. The reminder is scheduled seven calendar days before. If approval occurs after either threshold, production should send the reminder immediately if overdue and make the request available as soon as the five-day window is reached; never backdate a notification or issue a certificate before eligibility.
