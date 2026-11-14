# ILVORA Workforce – Branch Admin / HR Service 4: Leave Management

## Prototype v1 features
- Branch leave overview and approval queue.
- Leave application list and review/routing screen.
- Medical and casual leave policy and approval authority matrix.
- Paid medical leave can be approved by Head Office only; Branch Admin/HR can verify and recommend but cannot grant paid status.
- Five approved paid medical-leave days per employee per year; additional medical leave is unpaid.
- Casual leave is unpaid; Branch Admin/HR may approve up to five days under delegated authority.
- Any leave exceeding five days routes to Head Office.
- Final approved leave updates attendance and payroll in the intended production workflow; pending/rejected leave does not.
- Approved leave application printing only. Pending, returned or rejected applications cannot be printed as approved records.
- Printed approved form includes application reference, Employee ID, leave dates, leave type, paid/unpaid status, approver, authority, approval date and signature spaces.
- Physical filing reference field for printed approved records.

## Important workflow clarification
Leave applications are submitted and reviewed digitally. Printing becomes available only after final approval. A pending or rejected application cannot be printed from the Approved & Print section.

## Prototype limitations
This is a front-end demo with illustrative data. The Head Office decision button is a simulation only and is not a live approval. No real employee database, document storage, notification, attendance or payroll integration is connected. Do not enter real employee medical or personal information.

## Production requirements
- Enforce role permissions server-side; paid medical leave approval must be restricted to Head Office.
- Track annual paid medical-leave balance by approved leave dates and policy year; prevent concurrent approvals from exceeding the five-day allowance.
- Branch Admin/HR can verify and recommend medical leave but cannot grant paid status.
- Route any leave exceeding five days to Head Office; casual leave up to five days may be approved by Branch Admin/HR.
- Only final approved applications can produce the approved printable form. Print event should record who printed, when, version and physical filing reference.
- Approved leave records must update attendance and payroll through audited transactions; payroll closed periods require adjustment handling.
- Store medical certificates and leave attachments securely with least-privilege access and the agreed retention policy.
- Ensure rejected/pending applications remain non-printable as approved records.
