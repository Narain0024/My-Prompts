# Smart Payslip Manager — Monthly PDF Processing, Distribution & Reconciliation

- **Category:** Productivity & Automation
- **Provenance:** User-developed requirements dated 11 November 2026; reconstructed from conversation summary. Not a verbatim original.
- **Description:** Define a monthly payroll workflow that processes a combined payslip PDF, separates employee pages, distributes them securely, and reconciles payroll data.
- **Purpose:** Reduce repetitive payroll administration while adding validation, approval, and reconciliation safeguards.
- **Tags:** `payroll`, `payslip`, `pdf-splitting`, `whatsapp`, `reconciliation`, `employee-data`

## Copy-ready prompt

```text
Act as a senior payroll product architect, automation engineer, and security-focused full-stack developer.

Design and implement a Smart Payslip Manager for monthly payroll operations.

## Known workflow requirements
- The monthly input is a PDF.
- The PDF may contain payslips for multiple employees.
- The system must identify and split the combined PDF into one employee-specific PDF per person.
- The system should support secure distribution of each payslip to its intended employee through WhatsApp, with an appropriate accompanying message.
- The system must include monthly payroll reconciliation.

Treat any unspecified WhatsApp provider, employee matching method, approval workflow, and reconciliation source as design decisions to clarify or present as explicit options. Do not assume access to a WhatsApp account or API.

## 1. PDF ingestion and processing
- Accept the monthly combined payslip PDF.
- Detect employee boundaries and extract the relevant employee identifier and pay period where possible.
- Split the document into individual employee PDFs.
- Preserve page order, readability, and document integrity.
- Flag pages that cannot be confidently matched rather than assigning them by guesswork.

## 2. Employee matching and distribution
- Maintain or import an employee directory with unique employee identifiers and approved contact details.
- Match each generated PDF to exactly one employee.
- Provide a review screen for uncertain matches.
- Prevent duplicate sends.
- Require an authorized approval step before sending payslips.
- Keep a delivery log with employee, pay period, timestamp, status, and failure reason without exposing unnecessary salary details.
- Send only the intended employee's document to the corresponding recipient.
- Support a configurable WhatsApp message template.

## 3. Monthly payroll reconciliation
Design a reconciliation workflow that compares the payroll source data with the generated payslips and the monthly distribution register.

At minimum:
- Compare employee counts and employee identifiers.
- Compare gross earnings, deductions, and net pay when structured payroll data is available.
- Identify missing employees, duplicate records, mismatched amounts, missing payslips, and unexpected records.
- Reconcile totals by pay period and relevant payroll component.
- Provide a clear exception report with expected value, actual value, variance, and resolution status.
- Preserve the source values and never silently overwrite payroll data.
- Allow authorized users to mark exceptions as reviewed or resolved with an audit trail.

If the only input is a PDF, explain which fields can be reliably extracted and which reconciliation checks require an additional payroll register or structured source file. Do not claim a full financial reconciliation can be performed from incomplete data.

## 4. Security and privacy
- Apply role-based access to employee and payroll information.
- Protect uploaded PDFs, extracted data, and generated payslips.
- Avoid public links and accidental cross-employee access.
- Keep audit logs for imports, edits, approvals, reconciliation, and delivery.
- Define retention and deletion controls.
- Never expose credentials, API tokens, or private employee data in logs or repository files.

## 5. User experience and reporting
Provide a monthly dashboard showing:
- Import and processing status.
- Total employees detected.
- Payslips generated.
- Items requiring review.
- Reconciliation status and exceptions.
- Distribution status and failures.

Generate a downloadable monthly reconciliation report and a distribution summary.

## 6. Architecture and implementation
Before coding, deliver:
1. Requirements and assumptions.
2. End-to-end workflow.
3. Architecture and technology choices.
4. Data model and employee-matching strategy.
5. PDF extraction and splitting approach.
6. WhatsApp integration options and prerequisites.
7. Reconciliation logic and exception rules.
8. Security model.
9. Testing strategy.
10. Phased development roadmap.

Then implement in stages. Include tests for PDF splitting, employee matching, duplicate prevention, reconciliation calculations, approval gates, and delivery failure handling.

Do not send real payslips or connect to a live messaging service until I explicitly configure and approve the integration.
```

## Customization

- `{{PAYROLL_PERIOD}}`: month and year.
- `{{EMPLOYEE_DIRECTORY_SOURCE}}`: approved employee master source.
- `{{RECONCILIATION_SOURCE}}`: payroll register, bank file, HRMS export, or other source.
- `{{WHATSAPP_PROVIDER}}`: approved WhatsApp Business API/provider.
- `{{APPROVAL_ROLES}}`: who can review and authorize distribution.

## Source notes

The 11 November 2026 conversation summary confirms PDF monthly input, individual PDF splitting, WhatsApp distribution, and monthly payroll reconciliation. The prompt above adds explicit safety and data-integrity requirements as a labelled reconstruction; verify these details against the original conversation before treating them as user-authored source wording.
