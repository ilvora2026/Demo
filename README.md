# ILVORA Workforce – Employee Service 6 Prototype v2

## Added in v2
- Policy acknowledgement now requires reading the policy, ticking a mandatory agreement declaration, and entering an OTP.
- OTP is generated in the demo and notionally delivered to both the employee's registered mobile number and registered email address.
- Acknowledgement is recorded only after the checkbox is selected and OTP matches.
- Branch Admin / HR can view acknowledged policy records and download or print the policy together with employee acknowledgement evidence.
- Record includes employee number, branch, policy title/version, agreement wording, acknowledgement timestamp and masked contact channels.

## Demo test
1. Open `index.html` in a modern browser.
2. As Employee, open Company Policies and select "Read policy & acknowledge".
3. Click "Send OTP to registered mobile & email".
4. For this front-end demonstration only, the OTP is displayed on screen. Tick the agreement checkbox, enter the displayed OTP, and verify.
5. Switch preview role to Branch Admin / HR and open HR Policy Records.
6. Download or print the acknowledged policy record.

## Important limitations
Front-end prototype only. OTP is generated locally and is NOT sent by SMS or email. Do not use the displayed demo OTP as a security mechanism. Data is in browser memory and resets on refresh. No real authentication, secure document storage, server-side acknowledgement, audit immutability, or notification delivery is implemented.

## Production requirements
- Generate OTP server-side using a cryptographically secure random generator.
- Deliver OTP to both verified registered channels (SMS and email); apply short expiry, attempt limits, resend cooldown, rate limiting and one-time use.
- Verify the agreement checkbox and OTP on the server before committing acknowledgement.
- Record employee identity, policy/version, exact declaration text/version, timestamps, delivery/verification outcome and audit metadata.
- Preserve the exact policy document/version acknowledged.
- Provide Branch Admin / HR read-only access to download and print acknowledgement records, scoped to their branch; Head Office access according to permissions.
- Ensure acknowledgement does not unlawfully waive statutory rights or replace separate legally required consent/training. HR/legal should approve declaration wording and policy contents.
