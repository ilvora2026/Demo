# ILVORA Workforce — Employee Service 2: My Attendance

## Prototype features
- Monthly attendance summary
- Today's shift and punch overview
- Attendance history
- Employee attendance correction request
- Correction request history and simulated pending HR review
- Attendance information and audit-trail principles

## Workflow
Employee views own records -> submits correction request -> Branch Admin / HR reviews -> authorised decision is recorded -> employee can view the result. Original punches should remain preserved; approved corrections must be auditable.

## Important limitations
Front-end demo with sample data only. No real authentication, GPS, QR scanner, biometric device integration, backend attendance capture, database, notifications, approval engine or server-side permissions. The form simulates a correction request in the browser.

Attendance grace periods, checkout extension, QR/GPS validation and photo retention are intentionally not hard-coded here; they must be confirmed against the final attendance policy before implementation.

Open index.html in a modern browser.
