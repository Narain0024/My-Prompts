# Prompt Quality Standard

Score each proposed prompt from 0–2 on each criterion.

| Criterion | 0 | 1 | 2 |
|---|---|---|---|
| Objective | Missing | Broad | Specific and testable |
| Context | Missing | Partial | Sufficient to understand the task |
| Instructions | Vague | Some structure | Clear, ordered, actionable |
| Constraints | Missing | Some included | Important boundaries explicit |
| Output format | Missing | Implied | Explicit and usable |
| Reusability | One-off | Some placeholders | Clearly adaptable |
| Verification | None | Basic review | Includes validation / quality checks |

**Suggested acceptance threshold:** 10/14, with no zero for objective, constraints, or output format.

A high score does not override provenance. A reconstructed prompt must remain labelled reconstructed even if it is excellent.

## Good prompt practices

- State the role only when it improves the task.
- Put the main objective near the beginning.
- Separate context, instructions, constraints, and expected output.
- Use placeholders such as `{{INPUT_FILE}}` or `{{TARGET_AUDIENCE}}`.
- Define how uncertainty, missing data, and errors should be handled.
- Require verification for tasks involving calculations, files, code, or changing facts.
- Avoid contradictory requirements and unnecessary verbosity.
- Never invent source details to make a prompt appear complete.
