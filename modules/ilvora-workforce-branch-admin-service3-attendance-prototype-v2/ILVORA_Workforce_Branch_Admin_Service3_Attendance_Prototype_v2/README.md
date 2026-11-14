# ILVORA Workforce – Branch Admin / HR Service 3: Attendance Management

## Included in prototype v1
- Branch-scoped attendance overview and KPI summary.
- Daily attendance register with department filter, print and demo CSV export.
- Attendance Marker / Kiosk workflow integrated into Branch Admin / HR.
- Separate Attendance Operator permission boundary: can assist with check-in/check-out but cannot edit punches, approve corrections, access payroll/bank details or manage HR records.
- Attendance exception review for late arrival, early checkout, missed punch and no punch.
- Branch Admin/HR review notes that do not modify original punches.
- Formal correction request submission to Head Office with employee, date, original record, requested correction, evidence reference and reason.
- Head Office approval remains mandatory; Branch Admin/HR cannot approve. No attendance changes before approval.
- Reports and payroll attendance closure workflow, reflecting the agreed attendance closure after the 20th.
- Preserves original punch and audit trail concept; payroll-closed changes require payroll adjustment rather than silent edits.

## Prototype limitations
This is a front-end demonstration using illustrative data. It is not connected to employee records, roster, GPS, QR, OTP, face recognition, cameras, SMS/email, Cloudflare D1, payroll or authentication. Kiosk punch actions, reports and correction submissions are simulated in the browser only. Do not enter real employee personal, biometric or payroll information.

## Production requirements
- Enforce branch scoping and role permissions server-side.
- Verify identity and authorised device/session; secure rotating QR, OTP and any biometric processing with lawful basis and privacy controls.
- Attendance Operator must have only the minimum kiosk permission; dual-role users need explicit separate permissions.
- Immutable punch events; no direct edits/deletions. Record device, timestamp, verification outcome and audit metadata.
- Branch Admin/HR submits correction requests; Head Office reviews and approves/rejects/returns; requester cannot approve own request.
- On approval, append an auditable correction while retaining original punch; notify employee and Branch Admin/HR.
- If payroll is closed, create an adjustment workflow.
- Retain/delete attendance photos and records according to the previously agreed retention schedule and applicable law; preserve legal holds and physical print/filing register.
- Confirm exact grace-period, early/late punch and shift-boundary rules before production configuration.


## Updated in v2 – Attendance retention and reminders
For each attendance month:
- Detailed attendance register must be printed and physically filed by the 15th of the following month.
- Print reminders begin on the 10th (5 calendar days before the deadline) and continue until the print/filing register confirms completion.
- Detailed digital attendance report is scheduled for deletion after the 21st of the following month.
- Deletion reminders begin on the 16th (5 calendar days before the deletion date) and continue until deletion is completed or an authorised hold is recorded.
- Brief attendance summary is retained for 3 years, then automatically deleted after its individual expiry date. Summary expiry reminders begin 5 calendar days before expiry.
- Notifications go to Branch Admin/HR and the Head Office records custodian, with overdue escalation.
- Legal, litigation, investigation, audit or regulatory holds pause deletion. Holds must be authorised and recorded.
- The physical detailed register is governed by its separate approved physical-record retention and secure-destruction schedule; digital detailed-report deletion does not authorise destruction of printed records.

Prototype v2 displays the policy, dates, reminders preview and monthly status controls. It does not send real notifications, execute scheduled deletion or create secure physical print records. Production requires server-side scheduled jobs, role-based notification delivery, immutable deletion/print logs, legal-hold checks, and an approved retention schedule reviewed by HR/legal/compliance.
