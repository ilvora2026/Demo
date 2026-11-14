ILVORA WORKFORCE – SIGNATORY, PAYROLL & EXPERIENCE CERTIFICATE PROTOTYPE v1

Open index.html in a modern browser.

FEATURES
1. Administrator signatory setup:
   - Configure one or two Managing Director names.
   - Upload each MD's own separate signature image.
   - Upload company seal image.
   - If only one MD is configured, generated document preview shows only that MD.
   - If two MDs are configured, both names and signatures are shown.
   - A signature image cannot be configured without its corresponding name.

2. Payroll:
   - Payslip preview with employee, position, department, month, earnings, deductions and net pay.
   - Uses only the configured MD signature(s) and company seal.

3. Employee portal experience certificate request:
   - Request reference generated.
   - Certificate includes employee name, ID, position, department, employment start date, approved end date and calculated service duration in years, months and days.
   - Generation is blocked unless MD-approved resignation, passed last working day and completed company clearance are confirmed.
   - Preview includes configured MD signature(s) and company seal.

IMPORTANT GOVERNANCE / SECURITY
- The uploaded MD names/signatures and company seal are restricted by design to automatically generated payslips and experience certificates. Do not use these assets on other documents.
- The prototype's setup, uploaded images, requests and generated previews are browser-session demonstrations only.
- No real authentication, permission enforcement, secure storage, payroll engine, HR database, automated trigger, email delivery or employee portal backend is connected.
- Production implementation must store signatory and seal assets in private access-controlled storage, restrict setup changes to specifically authorised roles, record approvals and audit history, and protect the assets against unauthorised download or reuse.
- A production experience certificate should be automatically generated only after the approved last working day has passed and all required exit clearances are complete. The employee can request it through the portal; the system should also be able to trigger generation automatically when all conditions become true.
- Employment duration calculation should use validated employment dates and the organisation's approved inclusive/exclusive date-counting policy. The demo uses calendar year/month/day difference.
- Payslips should be generated from approved payroll records and payroll cycle, not manually entered demo values.
- Confirm applicable legal and company requirements for signatory authority and certificate wording before production use.

All sample data is illustrative. Do not upload real signature/seal images or personal data to this demo.

UPDATED v2 RULES:
- Employee certificate request window opens 5 calendar days before the approved last working day.
- Automated reminder scheduled 7 calendar days before the approved last working day.
- Certificate generation remains blocked until the approved last working day has passed and all company exit clearances are complete.
