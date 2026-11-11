# Prompt Library Curation from Conversation History

- **Category:** AI & Prompt Engineering
- **Provenance:** User-authored source request (11 November 2026); polished for repeat use
- **Description:** Audit accessible ChatGPT conversation records, select meaningful reusable prompts, improve their structure, and prepare a maintainable GitHub library.
- **Purpose:** Build a curated archive without pretending inaccessible conversations were reviewed.
- **Tags:** `prompt-engineering`, `conversation-audit`, `knowledge-management`, `github`, `markdown`

## Copy-ready prompt

```text
# Prompt Library Curation from ChatGPT Conversation History

Review the ChatGPT conversation history and conversation files that are actually accessible to you. Identify prompts that I explicitly wrote or meaningfully developed with you, and prepare a curated, GitHub-ready prompt library.

## 1. Scope and source verification
- Review all history and files available through the tools and context you can genuinely access.
- Do not claim to have reviewed my entire account if only a subset is available.
- Record the source conversation/date when available.
- Distinguish user-authored prompts, collaboratively refined prompts, assistant-generated drafts accepted by me, and reconstructed prompts.
- Never present reconstructed wording as a verbatim original.

## 2. Selection
Include prompts that have a clear objective, useful context, actionable instructions, important constraints, and an expected output.
Prioritize reusable, detailed, practical prompts.
Exclude casual questions, ordinary messages, incomplete follow-ups, terminal output, and one-off troubleshooting unless they form a meaningful reusable workflow.
When a prompt has multiple iterations, retain the most complete confirmed version and preserve the original when substantial changes were made.
Do not merge unrelated prompts.

## 3. Editing
Correct spelling, grammar, formatting, and unclear wording.
Improve clarity and instruction order without changing intent or removing constraints.
Replace context-specific values with clearly marked placeholders when doing so preserves the task.
If the original wording is unavailable, create a clearly labelled reconstruction only when the recorded requirements are sufficient; otherwise place the candidate in a review queue.

## 4. Organization
Create one Markdown file per selected prompt. Each file must contain:
- Title and category
- Description and purpose
- Provenance and source date/reference
- Complete copy-ready prompt
- Placeholder guidance
- Tags
- Change log where useful

Create a professional README.md, searchable INDEX.md, CONTRIBUTING.md, PROMPT-QUALITY-STANDARD.md, and REVIEW-QUEUE.md.
Use lowercase kebab-case filenames and a scalable category structure.

## 5. Quality control
- Detect exact and near-duplicate prompts.
- Count discovered candidates, selected prompts, duplicates removed, and prompts polished.
- Explain how counts were determined and avoid false precision where the history is incomplete.
- Keep incomplete or ambiguous candidates in a separate review list.
- Verify that every index entry points to an existing file.
- Check that no private data, credentials, or confidential content is exposed.

## 6. Deliverables
Provide the repository folder structure, all individual Markdown files, README, index, review queue, and a concise inventory with transparent counts.
Package the collection as a ZIP if file creation is available.

Do not upload to GitHub, modify a remote repository, or publish anything without my explicit approval.
```

## Customization

- Replace “ChatGPT” if auditing another assistant's export.
- Add a date range only when you want a bounded audit.
- Add preferred categories to the repository structure.
- Keep the no-publication-without-approval constraint.

## Source notes

Based on the user's detailed request on 11 November 2026. The source request itself is preserved in substance; this file is a cleaned reusable edition.

## Change log

- 2026-11-11: First reusable edition.
