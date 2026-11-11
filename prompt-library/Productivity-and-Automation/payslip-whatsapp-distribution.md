# Secure Payslip Distribution via WhatsApp

- **Category:** Productivity & Automation
- **Provenance:** Reconstructed / polished from a payslip-distribution request associated with the pinned-chat material titled “POLISH” and related payroll discussions; exact original wording was not available.
- **Use case:** Design a secure, auditable workflow for distributing individual employee payslips through WhatsApp.
- **Tags:** `#payroll` `#payslip` `#whatsapp` `#privacy` `#automation`

## Copy-ready prompt

Act as a senior payroll automation architect and security-conscious software engineer. Design a reliable workflow to distribute monthly employee payslips through WhatsApp.

Assume the source may include a combined PDF containing multiple employees' payslips and a separate Excel/CSV file containing employee identifiers and WhatsApp contact numbers. Treat these as inputs to validate, not as automatically trustworthy data.

Design the workflow to:
1. Accept the monthly payslip PDF and employee contact file.
2. Extract and split the combined PDF into one employee-specific PDF per person.
3. Match each payslip to an employee using a deterministic identifier, not name-only fuzzy matching.
4. Validate employee identifiers, page ranges, contact numbers, duplicate records, missing payslips, and unmatched documents.
5. Require a human review/approval step before any message is sent.
6. Send each employee only their own payslip using an approved WhatsApp Business integration and compliant message templates where required.
7. Prevent cross-employee disclosure, duplicate sends, accidental group delivery, and sending to unverified numbers.
8. Record delivery status, timestamps, failures, retries, and operator actions in an audit log without unnecessarily storing sensitive document contents.
9. Protect files in transit and at rest, restrict access, define retention/deletion rules, and handle credentials securely.
10. Produce a reconciliation report showing total employees, matched payslips, sent, delivered, failed, skipped, and pending approvals.

Explain the architecture, data model, validation rules, failure handling, privacy/security controls, operational costs, and implementation roadmap. Clearly distinguish what is technically possible from what depends on WhatsApp Business Platform approval, policies, templates, or provider capabilities.

Do not send messages or process real employee data during planning. Do not assume consent, authorization, or legal compliance; identify the approvals and policy checks required before production use.

## Customization

Specify monthly volume, source PDF structure, employee identifier, contact-file columns, WhatsApp provider, hosting environment, approval roles, retention period, and applicable jurisdiction.
