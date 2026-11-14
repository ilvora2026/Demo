# ILVORA Workforce — Employee Service 1

## Confirmed design decisions
- Profile photo: HR upload/management only. Employee cannot upload or replace the photo.
- Personal information: all changes submitted as requests and require authorised HR approval before the central record changes.
- Employee IDs: branch-specific, permanent and never reused.

## Proposed branch ID prefixes
- Head Office: ILV-HO-001
- Neelambari Hospital, Thamarakulam: ILV-NH-001
- ILVORA Health Clinic, Kottarakkara: ILV-KK-001

These prefixes are proposals for approval. Each branch has its own sequence; the full ID remains globally unique.

## Prototype contents
Personal profile, employment details, document visibility concept, profile-change request form and simulated pending-approval history.

## Important limitations
This is a front-end demo with sample data only. It has no real authentication, database, secure file storage, photo upload, backend HR approval, audit log, or server-side permission enforcement. The request form only simulates a request in the browser. Production requires authenticated APIs, database-backed approval workflow, branch-scoped access controls, audit logging and secure document storage.

Open index.html in a modern browser.
