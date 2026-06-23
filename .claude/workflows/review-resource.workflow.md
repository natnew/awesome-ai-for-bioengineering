# Workflow: review-resource

Review a suggested resource and decide accept, reject, or revise.

## Steps

1. Read the suggestion (issue or pull request).
2. Run `resource-entry-review` for fit, signal, placement, and description.
3. Run the source-quality-reviewer for canonical link, credibility, and duplicates.
4. Run `safety-boundary-reviewer` for unsafe detail or overclaiming.
5. Decide:
   - **Accept** — provide the final entry and section.
   - **Revise** — request specific changes (link, description, section).
   - **Reject** — give a short, respectful reason.

## Rules

- Minimise contributor friction: accept safe, useful submissions; request changes only when needed.
- Keep feedback concise and specific.
- Do not commit or push unless explicitly instructed.
