ILVORA WORKFORCE
Head Office Admin Panel – Service 10: Branch Management & GPS Location Setup
Prototype v1

RUN
1. Extract this ZIP.
2. Open index.html in Chrome or Edge.
3. Add a branch using its name, location, address, type, Google Maps link/coordinates and geofence radius.
4. Paste a full Google Maps URL or raw latitude, longitude and select "Extract coordinates".
5. Verify the coordinates and open the point in Google Maps before saving.
6. Review the branch register, edit an entry, and try the sample employee branch assignment.
7. Export the branch register as CSV or print the page.

FEATURES
- Head Office branch creation and editing.
- Branch name, location, full address and type (Clinic, Hospital, Pharmacy, Laboratory, Other).
- Google Maps coordinate extraction from common full URL formats and raw latitude/longitude.
- Per-branch configurable geofence radius (demo validation: 10–2,000 metres).
- Branch register with coordinates and Google Maps links.
- Sample employee-to-branch assignment workflow.
- Demo location/branch change audit history.
- CSV export and print/Save PDF.

GOOGLE MAPS LINK SUPPORT
The prototype attempts to parse coordinates from common URL formats such as:
- https://www.google.com/maps/@9.12345,76.12345,17z
- URLs containing ?q=9.12345,76.12345
- URLs containing !3d9.12345!4d76.12345
- Raw text: 9.12345, 76.12345

Shortened share URLs (such as maps.app.goo.gl) usually do not contain coordinates in the pasted text. This offline prototype does not resolve redirects. Open the short link in Google Maps, copy the full URL or coordinates, then paste them here. Production can resolve supported short links server-side and/or use a geocoding service.

IMPORTANT PRODUCTION LIMITATIONS
- This is a front-end demo. Branches, assignments and audit entries are held only in browser memory and reset on refresh.
- It is not connected to Cloudflare D1, a live employee directory, Google Maps API, geocoding service, mobile GPS or attendance hardware.
- The prototype cannot capture or validate an employee's live device location, calculate live geofence entry, or prevent GPS spoofing.
- Saving a branch does not by itself activate live attendance validation.

PRODUCTION INTEGRATION REQUIREMENTS
1. Persist branch records in Cloudflare D1 with unique branch IDs and server-side validation.
2. Resolve Google Maps short links securely on the server, validate allowed URL hosts, and extract or geocode coordinates.
3. Require Head Office authorisation for create/update and retain immutable before/after audit events.
4. Store a configurable geofence radius for each branch.
5. Link every employee's active branch assignment and effective date to the branch geofence.
6. At check-in/out, capture permissioned device GPS, timestamp and accuracy; validate distance from the assigned branch coordinates on the server.
7. Define GPS accuracy thresholds, mock-location/spoofing controls, offline handling, exceptions and manual review.
8. Treat GPS as one attendance signal, not proof of identity. Keep QR/OTP or other approved controls separate.
9. For temporary duty or branch transfer, use approved time-bound assignments and audit the change.
10. Apply privacy minimisation, access controls, retention limits and employee notice/consent requirements after legal review.

Do not enter real employee personal data into this prototype.
