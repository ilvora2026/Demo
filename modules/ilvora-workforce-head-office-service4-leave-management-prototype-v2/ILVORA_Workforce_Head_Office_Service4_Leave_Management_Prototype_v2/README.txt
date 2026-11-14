ILVORA Workforce – Head Office Admin Panel
Service 4: Leave Management & Central Approval – Prototype v2

New in v2:
- Detailed and brief leave reports
- Reports downloadable by individual branch or as a common consolidated report
- Date-range selection
- CSV download compatible with Excel
- Print / Save as PDF workflow
- Document cleanup policy after printing:
  * Temporary or duplicate uploads may be deleted only after successful print and filing confirmation.
  * Medical certificates and legally required leave evidence are retained digitally for 5 years, subject to legal review.
  * Printing does not authorise deletion of retained evidence.
  * Legal, audit or investigation holds pause deletion.
- Physical print register and secure filing reminders

Existing workflow:
- Head Office approval for all paid medical leave
- Maximum 5 paid medical-leave days per employee per year; excess medical leave unpaid
- Casual leave unpaid; Branch Admin / HR can approve eligible requests up to 5 days
- Leave exceeding 5 days is routed to Head Office
- Pending, returned or rejected requests do not change attendance/payroll

Important:
This is a front-end demo using illustrative records. CSV export and print layout work locally in the browser. PDF is created through the browser print dialog using Save as PDF. It is not connected to Cloudflare D1, live employee records, secure file storage, print verification, notifications, or scheduled deletion. Production must implement authenticated exports, print-register logging, server-side retention controls, legal holds, secure document storage, and audit logs.
