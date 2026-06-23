# Workflow: review-safety-boundaries

Inspect `README.md` for unsafe detail, overclaiming, or inappropriate resources.

## Steps

1. Read every entry and its description.
2. Run `safety-boundary-reviewer` against the safety rules in `SECURITY.md` and `.github/instructions/safety-boundaries.instructions.md`.
3. Flag any entry that includes or implies wet-lab protocols, pathogen engineering, genetic-manipulation procedures, synthesis routes, or other operational biological detail.
4. Flag overclaiming or hype that a source cannot substantiate.
5. For each flag: generalise the description, or recommend removing the resource if it is out of bounds.
6. Confirm dual-use resources are framed around responsible release or controlled access.

## Rules

- Never add unsafe detail in the output.
- Preserve high-level AI engineering usefulness.
- Do not commit or push unless explicitly instructed.
