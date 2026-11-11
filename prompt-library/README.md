# Personal Prompt Library

A curated, versionable collection of reusable prompts for AI-assisted work, software development, robotics, analytics, productivity, and professional communication.

> **Collection provenance:** This first edition was assembled from conversation context, retrieved conversation summaries, and a limited set of exported conversation files available in this workspace on 11 November 2026. It is not a verified export of every ChatGPT conversation in the account. Prompts whose exact original wording was unavailable are labelled as reconstructed or polished; no missing source text is represented as a verbatim original.

## Goals

- Preserve prompts that solve meaningful, repeatable problems.
- Keep prompts readable, reusable, and easy to adapt.
- Distinguish user-authored source material from assistant-assisted refinements.
- Improve prompts through explicit versioning rather than silently overwriting intent.

## Repository structure

```text
prompt-library/
├── README.md
├── INDEX.md
├── CONTRIBUTING.md
├── PROMPT-QUALITY-STANDARD.md
├── REVIEW-QUEUE.md
├── AI-Prompt-Engineering/
│   ├── prompt-library-curation.md
│   └── smart-prompt-organizer-concept.md
├── Career-and-Professional-Development/
│   └── fresher-resume-strategy-and-builder.md
├── Creative-Design/
│   ├── birthday-zine-creative-brief.md
│   └── robotics-hiring-poster.md
├── Personal-Communication/
│   └── cute-flirty-message-polisher.md
├── Robotics-and-Education/
│   └── robotics-kit-label-system.md
├── Software-Development/
│   └── smart-prompt-organizer-ui-redesign.md
├── Productivity-and-Automation/
│   ├── payslip-generator.md
│   ├── payslip-whatsapp-distribution.md
│   └── smart-payslip-manager.md
└── Technology-Comparisons/
    └── smartphone-comparison-review.md
```

## How to use a prompt

1. Open the relevant Markdown file.
2. Read its purpose, provenance, and customization notes.
3. Replace every `{{PLACEHOLDER}}` with your actual context.
4. Keep constraints that matter to the task; remove only irrelevant optional instructions.
5. Save meaningful improvements as a new version or update the change log.

## Prompt file convention

Use lowercase kebab-case filenames:

`descriptive-task-name.md`

Each prompt file should contain:
- Title and category
- Provenance / source status
- Description and use case
- Copy-ready prompt
- Placeholders and customization notes
- Tags

## Quality and provenance

This repository uses three provenance labels:

- **User-authored:** the source prompt was written by the user and its wording is available.
- **User-developed / collaboratively refined:** the user supplied the goal and material requirements; the final wording may have been refined with the assistant.
- **Reconstructed / polished:** the source intent is supported by conversation records, but the exact original prompt was not recoverable. This is not a verbatim transcript.

Do not claim that a prompt is verbatim unless the source text has been checked.

See [PROMPT-QUALITY-STANDARD.md](PROMPT-QUALITY-STANDARD.md) and [CONTRIBUTING.md](CONTRIBUTING.md).

## Current collection status

The current library contains **12 selected prompt files**: 6 from the initial pass and 6 additional reconstructed/polished candidates found in the pinned-chat material titled “POLISH”. The POLISH additions are explicitly marked as reconstructed because their exact original wording was not available. The inventory remains non-exhaustive; see [REVIEW-QUEUE.md](REVIEW-QUEUE.md) for topics that still need source-text verification.

## License

Choose a license before publishing. If the repository contains only your original prompt writing, a permissive documentation license may be appropriate; review any third-party or assistant-generated material before selecting one.
