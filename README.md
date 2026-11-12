# ILVORA Workforce – Attendance Correction Prototype v1

## Included
- Employee mobile attendance concept (personal registered phone or authorised branch kiosk).
- Attendance Marker kiosk operations and punch monitoring. No correction permissions.
- Branch Admin / HR correction request submission using employee number, branch, date, existing attendance, requested correction, reason and evidence reference.
- Head Office approval queue with approve, reject and return-for-clarification actions.
- Demonstration of approved record update and notifications to employee and Branch Admin / HR.
- Original attendance history and audit-preservation controls described in the interface.

## How to run
Open `index.html` in a modern browser. No installation is required.

## Demo instructions
1. Use the Preview role selector to switch between Employee, Attendance Marker, Branch Admin / HR and Head Office Admin.
2. As Branch Admin / HR, submit a correction request.
3. Switch to Head Office Admin and approve, reject or return the request.
4. Switch to Employee and Branch Admin / HR to view the resulting status.

## Important limitations
This is a front-end demonstration using in-memory sample data. Refreshing the page resets demo requests. It does NOT provide live login, GPS, camera/face recognition, QR token validation, OTP, secure device registration, database persistence, real Head Office approvals, audit-grade immutable logs, payroll recalculation or email/push notifications. The interface simulates the expected workflow only.

Production implementation must enforce permissions and approval on the server, preserve original attendance records, use secure audit logging, validate devices and QR tokens server-side, and send notifications only after a committed approval/update transaction. Any already-closed payroll period must use a controlled payroll adjustment workflow.
