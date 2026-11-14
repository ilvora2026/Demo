ILVORA WORKFORCE – FINAL INTEGRATED PROTOTYPE v1

START
1. Extract the ZIP.
2. Open index.html in Chrome, Edge or another modern browser.
3. Select a role, enter any non-empty demo username and password, and open the dashboard.
4. Open each service from its dashboard card. Service prototypes open in a new browser tab.
5. Use Switch role / Logout to return to the main portal.

INCLUDED ROLE DASHBOARDS
- Employee: 9 approved employee services + resignation/exit + signatory/experience certificate demo.
- Branch Admin / HR: 9 approved branch services + attendance correction + resignation.
- Head Office Admin: 11 approved Head Office services + resignation.
- Administrator: 15 approved Administrator services + resignation + MD signatory/payroll/experience certificate setup.
- Managing Director: executive command centre, visibility to all 15 Administrator services, resignation final approval and executive oversight.

BRAND
- Supplied ILVORA Healthcare logo used in portal header/background and app icon.
- Navy / teal / champagne-gold theme.

RESIGNATION RULES INCLUDED IN THE LINKED PROTOTYPE
- MD final approval is mandatory for every resignation.
- Certificate request opens 5 calendar days before approved last working day.
- Employee reminder is scheduled 7 calendar days before.
- Experience certificate generated only after approved last working day has passed and all company clearance is complete.
- All company access is to be disabled at 00:00 on the calendar day after the approved last working day, including employee portal, email, internal applications, SSO, VPN/remote access and physical access credentials where integrated.
- Historical and statutory records must be retained; access closure is not record deletion.

SIGNATORY RULES
- One or two MD signatories may be configured, each with a separate signature image.
- If one MD is configured, show one name/signature; if two are configured, show both.
- Company seal image is configured separately.
- MD signatures and seal are reserved only for automatically generated payslips and experience certificates.

IMPORTANT: THIS IS A PRE-IMPLEMENTATION FRONT-END AGGREGATION, NOT A LIVE DEPLOYMENT
- The portal's login is a demo navigation gate only. It does not authenticate users or enforce role permissions.
- Forgot-password OTP is simulated. No SMS/email OTP is delivered and no real password is changed.
- Each linked service is the latest available approved service prototype and retains its own demo behavior. They are linked from a common role portal but do not yet share one database or unified live workflow state.
- Cloudflare D1, Workers, GitHub deployment, live payroll, real attendance devices/GPS/face recognition, secure file storage, email/SMS, automatic scheduled access revocation, certificate notifications, and production audit logging are not connected.
- The resignation and exit automation schedules are specified in the prototypes; a production scheduler and identity-provider integrations are still required.
- MD executive command centre prototype was consolidated from the finalised dashboard structure but had not separately received explicit prototype approval before this combined build. Review it as part of this final prototype.
- Do not enter real employee, salary, medical, bank, identity, signature or other sensitive information into this demo.

NEXT IMPLEMENTATION PHASE (AFTER FINAL PROTOTYPE APPROVAL)
1. Review/approve combined portal and role navigation.
2. Reconcile shared data model, role permissions, branch scoping and audit events.
3. Implement Cloudflare Workers + D1 backend and secure object storage.
4. Implement authentication, OTP delivery, password reset, session control and role-based access.
5. Integrate notifications, scheduled certificate reminders, next-day access revocation, payroll and document generation.
6. Security, privacy, legal, payroll and HR acceptance testing.
7. Publish to the existing GitHub repository and configure production hosting only after explicit deployment approval.
