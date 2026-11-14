ILVORA Workforce — Administrator Service 13
Procurement, Inventory & Asset Management
Version 1 — Front-end demonstration

HOW TO RUN
1. Extract the ZIP.
2. Open index.html in a modern browser (Chrome or Edge recommended).

INCLUDED
- Procurement overview dashboard
- Branch purchase requisitions and register
- Vendor and quotation / purchase-order workflow concepts
- Goods receipt workflow concepts
- Branch stock, batch, expiry and reorder tracking
- Fixed asset register, maintenance and transfer concepts
- Reports, CSV export, print / Save as PDF
- Approval rules and role boundaries

IMPORTANT LIMITATIONS
This is a front-end prototype with illustrative sample data. It is not connected to Cloudflare D1, GitHub, authentication, email/SMS, vendor systems, accounting, payments, barcode scanners or live inventory. Browser changes are not persistently stored. File attachment, invoice storage, actual purchase order generation and server-side approvals are not implemented.

APPROVAL GOVERNANCE
- Branch Admin / HR raises requests and confirms receipt; cannot approve spending.
- Administrator reviews and may approve only within the procurement limit delegated by the Managing Director.
- Managing Director sets/revises the limit and approves above-limit purchases.
- Until a numerical limit is formally set, route all purchase commitments to the Managing Director.
- Do not split related orders to avoid approval thresholds; requester cannot approve their own request.

PRODUCTION CHECKLIST
Implement server-side role-based access, approval-limit enforcement, audit logs, vendor due diligence, quote comparison, budget checks, secure document storage, stock movement controls, batch/expiry/recall controls, asset tagging and transfer acknowledgements, backups, and an India/Kerala legal and financial retention schedule. For medicines and regulated products, validate applicable licensing, storage and traceability requirements before deployment.
