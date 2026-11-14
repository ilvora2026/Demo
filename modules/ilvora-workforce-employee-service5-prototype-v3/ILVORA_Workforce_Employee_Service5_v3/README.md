# ILVORA Workforce — Employee Service 5 v3: My Payslips & Payroll

## Included features (all requested)
1. Personal payslip history
2. Salary earnings and deductions breakdown
3. Secure payslip viewing concept
4. Payroll query submission
5. Payroll query history and status
6. Payroll schedule information
7. Employee salary-slip request by selected month
8. Mandatory Administrator approval before release
9. Employee request-status tracking
10. Downloadable approved payslip PDF concept
11. Automatic delivery to employee's registered email after approval

## Salary slip request workflow
Employee requests month -> Administrator reviews -> approve/reject -> approved PDF generated -> portal download enabled -> email sent to registered email -> status and delivery result recorded.

Security recommendation: send a secure, expiring authenticated download link in email rather than an unencrypted payslip attachment. The registered email should be read-only in this employee screen.

## Payroll schedule reflected
- Salary payment target: before the 12th of each month.
- Payslip generation target: 12th of each month.
- Attendance register closure: after the 20th.
These should be configurable by authorised payroll administrators.

## Important limitations
Front-end prototype with sample data only. The request form and query form simulate browser-side submissions. The download action creates a clearly marked sample PDF, not a real payslip. No real authentication, administrator approval, payroll integration, database persistence, email delivery, secure PDF generation or server-side authorization is implemented. Production requires authenticated APIs, employee-scoped access controls, audited approval, PDF generation, email service integration and delivery tracking.

Open index.html in a modern browser.
