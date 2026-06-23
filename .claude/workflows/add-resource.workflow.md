# Workflow: add-resource

Add one high-quality resource to `README.md`.

## Steps

1. Gather the candidate: name, URL, suggested section, type, and rationale.
2. Run `resource-entry-review` (and `paper-triage` or `benchmark-analysis` if relevant).
3. Verify the link is canonical, HTTPS, and live (source-quality-reviewer).
4. Run `safety-release-review` if the resource touches safety or dual-use.
5. Insert the entry into the correct section, preserving alphabetical order where practical.
6. Confirm no duplicate exists.
7. Recommend CI: awesome-lint, markdown link check, repository-health.

## Rules

- Add to `README.md` only. Do not create other files.
- One resource per change. Keep the description to one neutral line.
- Do not commit or push unless explicitly instructed.
