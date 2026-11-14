# ILVORA Workforce – Employee Service 9 Prototype v1
## My Requests & Helpdesk

### Included
- Create an employee service request.
- Employee ID and branch shown as read-only demo profile fields.
- Categories: HR/employment, letters/certificates, ID card, profile correction, IT/system support, facility/maintenance, equipment/supplies and other.
- Priority selection, subject, description, preferred contact method and optional attachment reference.
- Automatic demo request reference number.
- Personal request history, status, priority and last-updated date.
- Search and summary counts.

### Suggested workflow
Employee submits request -> system creates reference -> request is routed to the responsible service team -> authorised team reviews and assigns owner -> employee receives approved status updates -> team resolves request -> employee is notified and closure is recorded.

### Suggested routing
- HR / Employment, letters, ID cards and profile corrections -> Branch Admin / HR, with Head Office escalation where required.
- IT / System support -> authorised IT support.
- Facility / Maintenance and Equipment / Supplies -> authorised branch operations/facilities team.
- Other -> triage queue for authorised administrator.

### Production controls
- Employee can access only their own requests.
- Route by category, branch and service ownership; enforce access server-side.
- Keep internal notes and sensitive attachments hidden from employee view unless explicitly approved for release.
- Use secure file upload, malware scanning, size/type limits and access logging.
- Record request ID, creator, timestamps, assigned team/owner, status changes, messages, resolution and closure.
- Configure service-level targets, escalation reminders and overdue reporting.
- Avoid collecting passwords, patient-identifiable information or unnecessary sensitive data.
- Provide a separate emergency route for urgent safety incidents.

### Demo limitations
This is a front-end prototype. Demo employee details and sample requests are static. New requests exist only in browser memory and reset on refresh. No real login, database, file upload, ticket routing, email, SMS, notifications, SLA engine or backend permissions are connected.
