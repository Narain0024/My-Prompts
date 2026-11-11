# Bulk Payslip Generator from Employee Data

- **Category:** Productivity & Automation
- **Provenance:** User-authored objective; assistant-polished prompt reported in conversation record dated 17 October 2026. Exact full source wording was not reproduced in the available retrieval, so this is a faithful structured reconstruction.
- **Description:** Build an application that generates professional individual or bulk payslips from employee salary data.
- **Purpose:** Reduce manual payslip preparation while supporting validation, customization, and secure output.
- **Tags:** `payroll`, `payslip`, `excel`, `pdf`, `bulk-generation`, `privacy`

## Copy-ready prompt

```text
Act as an experienced payroll-systems analyst, product designer, and full-stack application developer.

Design and build a Payslip Generator Application that accepts employee salary data from an uploaded Excel file and generates professional payslips for one employee or an entire batch.

## Core requirements

### 1. Data import
- Accept an Excel workbook containing employee and salary information.
- Validate required columns and identify missing, malformed, or inconsistent values.
- Show clear row-level validation errors before generation.
- Allow the user to map spreadsheet columns to payslip fields when column names differ.

### 2. Payslip generation
- Generate a payslip for a single employee or multiple employees in one operation.
- Support configurable organization details, employee details, pay period, earnings, deductions, and net pay.
- Support flexible salary structures rather than assuming every employee has identical components.
- Provide a professional, customizable payslip template.
- Preview payslips before final generation.

### 3. Output
- Generate a separate PDF for each employee.
- Allow the user to download individual PDFs or a ZIP containing the batch.
- Use consistent, readable formatting and clear file naming.
- Ensure each employee receives only their own payslip.

### 4. Usability
- Provide employee search and filtering.
- Show import summaries, validation status, and generation results.
- Support correction and re-import without silently duplicating records.
- Make the workflow understandable to a non-technical payroll operator.

### 5. Privacy and reliability
- Protect employee salary and personal information.
- Avoid exposing one employee's information in another employee's output.
- Validate calculations and totals.
- Handle malformed files and generation failures gracefully.
- Do not log sensitive salary data unnecessarily.

## Before implementation
First provide:
1. Requirements analysis and assumptions.
2. Recommended architecture and technology stack.
3. Data model and spreadsheet schema.
4. Payslip layout approach.
5. Validation and calculation rules.
6. Security and privacy design.
7. Phased implementation roadmap.

Then implement the complete working application. Do not stop at a UI mockup: verify the import, validation, preview, PDF generation, batch ZIP export, and error-handling workflows with tests.
```

## Customization

- `{{INPUT_FORMAT}}`: Excel, CSV, or another approved source.
- `{{CURRENCY}}`: payroll currency.
- `{{PAYSLIP_TEMPLATE}}`: organization branding and layout.
- `{{OUTPUT_FORMAT}}`: individual PDFs, ZIP, or both.
- `{{DEPLOYMENT_TARGET}}`: local, internal server, or cloud.

## Source notes

Conversation context dated 17 October 2026 records a user-authored payslip-generator request with Excel upload, single/bulk generation, customizable template, separate PDFs/ZIP, validation, preview, search/filter, flexible salary structures, and privacy. The exact original text should be retrieved before claiming verbatim fidelity.
