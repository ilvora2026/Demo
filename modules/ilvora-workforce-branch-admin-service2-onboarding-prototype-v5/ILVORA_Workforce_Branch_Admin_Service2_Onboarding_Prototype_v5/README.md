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


## Added in v4 – Employee exit and access control
- Added an Employee Exit & System Access Control section to Employee Management.
- Termination: only the Administrator may revoke employee system access. Branch Admin/HR may record or submit the case but cannot revoke access.
- Resignation: once resignation approval and the last working day are recorded, employee login access is scheduled to be automatically disabled at the end of the last working day.
- Access revocation is not employee-record deletion. Employee profile, attendance, payroll, leave, payslips, signed contracts and audit records must be archived and retained under the approved retention schedule.
- Production implementation requires server-side role enforcement, approved-exit validation, scheduled server-side deactivation for resignations, session/token revocation, immutable audit events and safeguards against self-approval. A browser-only timer or client-side rule is not sufficient.
- The v4 prototype simulates the workflow; it does not connect to authentication, HR database, or a real scheduled deactivation service.


## Added in v5 – Separate Employee Enrolment page
- Added a dedicated Employee Enrolment page within Employee Management, separate from New Employee Onboarding.
- Intended for an already-approved employee with an existing permanent Employee ID. It does not create a new employee or generate an ID.
- Captures contact/address details, department/position, emergency contact and bank/payroll details; supports up to seven selected image/PDF documents in the demo.
- Includes save, print enrolment form and submit-to-Head-Office-for-verification demo actions.
- Salary remains Administrator-only and cannot be edited from the enrolment page.
- The prototype validates required fields, bank-account confirmation, IFSC format and the seven-file limit. It does not securely store or transmit data/files and does not connect to a real Head Office workflow.
- Production requires server-side employee/branch validation, least-privilege access, encryption, bank-data masking, secure document storage and scanning, audit logs, Head Office verification workflow, and approved physical/digital retention controls.
