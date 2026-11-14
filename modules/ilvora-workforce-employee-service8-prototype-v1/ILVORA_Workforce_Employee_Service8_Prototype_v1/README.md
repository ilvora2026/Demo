# ILVORA Workforce – Employee Service 8 Prototype v1
## Complaints & Grievances

### User decision
All complaints are identified submissions linked to the signed-in employee's employee ID. Anonymous submission is not included.

### Included in this prototype
- Complaint submission linked to employee ID and branch (demo profile).
- Complaint category, incident date, subject, detailed description, persons involved and optional evidence reference.
- Confidential-handling request and employee declaration.
- Complaint reference number generated on submission.
- Personal complaint history with status and last-updated date.
- Sample complaint records and search.
- Confidentiality and safety guidance.

### Proposed complaint workflow
Employee submits complaint -> system creates reference -> restricted authorised intake officer reviews -> impartial investigator is assigned -> investigation and evidence handling -> outcome/corrective action -> employee receives approved status/outcome communication -> closure or appeal route.

### Access and safeguarding rules for production
- Employee can submit and view only complaints linked to their own employee account.
- Branch Admin / HR must not automatically see all complaints.
- If a complaint concerns a Branch Admin, route it to Head Office or another independent authorised officer, bypassing the named person.
- If a complaint concerns Head Office HR, senior management or the normal escalation route, use a designated independent authority / board-level contact as approved by policy.
- Apply strict least-privilege access, case-level permissions, access logs and secure evidence storage.
- Keep investigator notes, witness statements and third-party personal information restricted; employee portal should show only approved updates.
- Protect against retaliation and provide an urgent safety/emergency reporting route for immediate risks.
- Define response timelines, investigation standards, appeal/escalation routes, retention and lawful disclosure rules with HR/legal review.
- Avoid collecting patient-identifiable information unless strictly necessary and lawfully authorised.

### Demo limitations
This is a static front-end demonstration. Sample data is held in browser memory and resets on refresh. It has no real authentication, file upload, notifications, case assignment, secure storage, investigation workflow, database or backend permissions. The displayed employee ID and branch are demo values.
