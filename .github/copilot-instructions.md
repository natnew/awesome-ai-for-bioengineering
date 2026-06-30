# Copilot instructions for natnew/awesome-ai-for-bioengineering

This repository is an Awesome List: curated links in README.md. Keep edits small, neutral, and focused on link quality, safety, and formatting.

Key checks for automated assistants

- Safety boundary: consult SECURITY.md before suggesting entries; never add procedural wet-lab or genetic-manipulation detail.
- Formatting: single-line bullets in README.md, alphabetical order within sections, HTTPS links, neutral descriptions.
- CI checks: run `npx awesome-lint` and `npx markdown-link-check README.md` locally or in CI.

Maintenance matrix (change -> required actions)

- README.md entries (add/edit/remove):
  - Ensure single-line bullet format and section placement.
  - Verify link resolves and is canonical.
  - Run `npx awesome-lint` and `npx markdown-link-check README.md`.
  - Update CONTRIBUTORS/all-contributors list only via the all-contributors workflow.

- CONTRIBUTING.md or SECURITY.md updates:
  - Update links in README and AGENTS.md references.
  - Run markdown link checks and mention changes in PR description.

- .github/workflows or CI changes:
  - Update `.mcp.json` if new services or runners are required.
  - Notify maintainers in PR description and include a short test run summary.

- Adding docs/ or major new files:
  - Add a short note to AGENTS.md describing location and purpose.
  - Add CI lint or link-check steps if documentation adds new pages.

How to run checks (recommended):

- npm/node present: `npm ci && npx awesome-lint && npx markdown-link-check README.md`
- without npm: `npx --yes awesome-lint && npx --yes markdown-link-check README.md`

Review guidance for PRs

- One resource per PR is preferred.
- Keep maintainer friction low: include canonical link, brief justification, and section for placement.
- If unsure about section choice, add a short note and tag maintainers.

Contact and conventions

- Default branch: main. Use feature branches and open PRs — do not push directly to main.
- Commit trailer: include `Co-authored-by: Copilot <223556219+Copilot@users.noreply.github.com>` when automated edits are produced by copilot tools.
