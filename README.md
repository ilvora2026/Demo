# ILVORA Workforce – Branch Admin / HR Service 2: Employee Onboarding

## Six-stage workflow
1. Branch Admin submits mandatory full name, address, position, mobile, Aadhaar, email, branch and department; PAN is optional, with up to seven PDF/image supporting documents.
2. Head Office verifies credentials and approves, returns for correction or rejects. Branch-specific Employee ID is generated only after approval.
3. Employee receives activation link and OTP at verified mobile/email. Username is Employee ID. OTP verification and mandatory password reset are required.
4. Branch Admin enters mandatory bank details and emergency contact details, then prints enrolment details.
5. After physical signing, Branch Admin uploads the signed employment contract against the Employee ID.
6. Head Office verifies the completed record and prints it for physical retention.

## Branch ID prefixes in prototype
- Head Office – Kochi: ILV-HO-###
- Neelambari Hospital – Thamarakulam: ILV-NH-###
- ILVORA Health Clinic – Kottarakkara: ILV-KK-###
Production IDs must be unique, permanent, atomic and never reused. The prototype simulates ID generation.

## Security / compliance
- Do not enter real Aadhaar, PAN, bank or employee information in this prototype.
- Review lawful purpose and necessity for Aadhaar collection; PAN collection under applicable Indian law and UIDAI requirements. Minimise data, encrypt at rest/in transit, mask ordinary displays, restrict access, and audit views/downloads/printing.
- Bank details require encryption and payroll/HR-only access; mask account numbers in general views.
- Production uploads require server-side file validation, malware scanning, secure storage, size/type limits and access logs.
- Head Office decisions must record verifier, timestamp, evidence checked and reason.
- OTP must be server-generated, time-limited, single-use, rate-limited and delivered through verified SMS/email. Never display OTP in production.
- Temporary credentials must be securely delivered; force password reset before access.
- Signed contracts must be versioned, linked to Employee ID and protected against silent replacement.
- Final verification and physical printing should create an audit/print register with retention and legal-hold controls.

## Demo limitations
Front-end simulation only. No real login, database, OTP delivery, email/SMS, secure file storage, server-side approval, or actual ID allocator. Demo OTP is displayed on screen for testing; uploaded files are not transmitted or retained. Browser print dialog is used for print actions.


## Added in v3 – Administrator-only fixed salary setup
- After Branch Admin submits the onboarding application, the Administrator enters the fixed monthly salary and effective date.
- Only the Administrator is authorised to enter, review, revise and save the salary. Branch Admin and Head Office do not receive salary-edit permissions.
- The demo requires a saved salary before Head Office can approve the application and generate the Employee ID.
- The saved fixed salary is linked to the employee onboarding record and is intended to become the base salary input for automatic payroll calculation.
- The demo keeps a simple in-session salary version history showing prior amount, editor label and timestamp. It resets on refresh and is not a secure audit log.
- Production must enforce Administrator-only access server-side, maintain immutable salary version/audit history, support effective dates and approved revisions, and integrate the active salary record with payroll. Payroll calculations must apply configured attendance, unpaid leave, deductions and statutory rules; do not treat fixed salary alone as the final payable amount.
- No real payroll database or salary permissions are connected in this prototype.
