# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

This repository is a public, maintained Awesome List for AI engineering in bioengineering, not an application codebase. There is no application build or runtime; the support files are limited to curation, contribution, review, CI, link quality, and agent operation. The `README.md` is the product.

Claude Code should read this file first, then use `AGENTS.md` as the shared, tool-agnostic operating protocol. Do not duplicate `AGENTS.md` here; this file is an orientation layer.

## North Star

- Preserve `README.md` as the canonical public artefact.
- Keep the list selective, durable, technically useful, neutral, and easy to scan.
- Help the maintainer make fast, consistent, low-friction decisions.
- Prefer small, precise edits over broad rewrites.
- Do not broaden the list beyond AI for bioengineering and the adjacent technical areas already represented in the README.

## Claude's Role

Claude may assist with:

- PR review
- Issue triage
- README entry review
- Broken-link investigation
- Duplicate detection
- Section placement
- Neutral description rewrites
- Safety-boundary review
- Maintainer comment drafts
- Small, safe maintainer edits when explicitly asked
- Improvements to agent instruction files when asked

Claude must not:

- Add entries without checking scope, safety, link quality, duplicates, and placement
- Invent facts about a resource
- Preserve promotional claims
- Add ranking, pricing, novelty, adoption, or performance claims without strong evidence
- Add any wet-lab, pathogen, genetic-manipulation, or synthesis detail (see Safety Boundary)
- Create content directories or category files outside `README.md`
- Rewrite the taxonomy or scope without explicit instruction
- Edit unrelated files
- Touch protected areas unless instructed
- Ask contributors to make trivial fixes the maintainer can safely make

## Repository Facts

- `AGENTS.md` contains the full tool-agnostic operating protocol.
- `CONTRIBUTING.md` contains contributor-facing rules and the entry format.
- `SECURITY.md` contains the safety boundary and out-of-scope content.
- `.github/instructions/` contains curation, link-and-source-quality, repository-maintenance, and safety-boundary guidance.
- `.github/PULL_REQUEST_TEMPLATE.md` contains contributor expectations.
- `README.md` is the primary and only content artefact: intro, a scope-and-safety note, Contents, the main sections, Contributing, and Contributors.
- README sections are single-line bullet lists. Match the surrounding section exactly.
- Entries take the form `* [Name](https://link) - Neutral, technically precise description.`
- Entries are kept in alphabetical order within a section where practical.
- One resource per pull request is preferred, with a short note on why it belongs.
- New categories or structural changes are handled separately from single-entry contributions.
- Protected areas include the Contents block, the intro and scope-and-safety note, the Contributors section and all-contributors markers, badges, and licence text.

## Always-Loaded Context

Keep this file short. It is an orientation layer, not a manual.

Use this routing:

- Need the full agent protocol → read `AGENTS.md`
- Need contribution rules → read `CONTRIBUTING.md`
- Need the safety boundary → read `SECURITY.md`
- Need curation, link, maintenance, or safety detail → read `.github/instructions/`
- Need style examples → inspect the target section in `README.md`
- Need contributor expectations → inspect `.github/PULL_REQUEST_TEMPLATE.md`
- Need maintainer precedent → inspect recent issues and merged PRs where available

Do not duplicate long sections from those files here.

## First-Pass Workflow

For any PR, issue, or README task:

1. Read the user request.
2. Read the relevant issue, PR, diff, or target README section.
3. Check the repository scope.
4. Check the Safety Boundary.
5. Check `CONTRIBUTING.md` if the task concerns a submission.
6. Check neighbouring entries for style, placement, and alphabetical order.
7. Search for duplicates.
8. Verify the link where tools allow.
9. Inspect the resource enough to understand what it is.
10. Choose the smallest useful action.
11. Produce a concise decision, edit, or maintainer comment.

## Entry Checklist

Before recommending acceptance or adding an entry, confirm:

- In scope for AI for bioengineering
- Technically useful
- Credible, canonical source
- HTTPS, durable link
- No duplicate or stronger existing equivalent
- Correct section, alphabetical where practical
- Local single-line bullet format matched
- Neutral description, no hype, no unsupported claims
- No avoidable tracking parameters
- No unsafe procedural detail
- No unnecessary new section

## Source Preference

Prefer:

- Official repositories
- Official documentation
- Papers (arXiv, DOI, publisher, or project page)
- Technical reports
- Benchmarks and datasets (official or maintained pages)
- Durable project pages
- Maintained tools and libraries

Treat cautiously:

- Launch posts and vendor pages
- Thin wrappers and link farms
- Newsletter and social posts
- Unmaintained repositories
- Pages dominated by sales language
- Time-sensitive comparisons

## Description Rules

Default pattern:

`* [Name](https://link) - Clear factual description.`

Descriptions should:

- Start with a capital letter
- End with a full stop
- Be short and specific
- Avoid title case
- Avoid starting with "A" or "An"
- Avoid marketing taglines
- Explain what the resource is, not why it is exciting

Remove or neutralise: "best", "latest", "most advanced", "powerful", "revolutionary", "cutting-edge", "leading", "fastest", and unsupported performance, adoption, maturity, or pricing claims.

## Safety Boundary (Hard Gate)

This is not a clinical, medical, laboratory, or experimental-protocol repository. The following must never enter the list, an entry description, an issue reply, or a PR comment:

- Wet-lab or experimental protocols
- Pathogen engineering or enhancement guidance
- Genetic-manipulation procedures
- Chemical or biological synthesis routes
- Any operational detail that could enable unsafe biological experimentation

Keep entries at the level of AI systems and what they model, predict, or generate. Responsible release and biosecurity resources are in scope at a high, governance-oriented level only. If a candidate drifts toward operational detail, generalise it or recommend declining, and flag the concern without restating the unsafe detail. See `SECURITY.md`.

## Section Placement

| Situation                             | Action                                                |
| ------------------------------------- | ----------------------------------------------------- |
| Exact fit in an existing section      | Place there.                                          |
| Fits two sections                     | Choose the narrowest accurate, most discoverable one. |
| Similar to neighbouring entries       | Place near those entries if local ordering allows.    |
| New theme with one entry              | Park, or place in the nearest broader section.        |
| New theme with several strong entries | Suggest a new section; do not create it unless asked. |
| Unclear placement                     | Explain the options briefly and recommend one.        |

## PR Triage

| Decision        | Use when                                                                                  |
| --------------- | ----------------------------------------------------------------------------------------- |
| Accept as-is    | Scope, safety, link, placement, format, and description are all sound.                     |
| Maintainer edit | Strong resource needing only minor wording, link, placement, or formatting fixes.         |
| Request changes | Relevance, evidence, link quality, or placement is materially unclear.                    |
| Close           | Out of scope, duplicate, promotional, broken with no replacement, or low technical value. |
| Park            | Promising but immature, needs a taxonomy decision, or needs maintainer judgement.         |

## Issue Triage

Suggestion issues:

- Strong, in scope, safe, canonical → draft entry and recommend acceptance.
- Strong but wording or placement needs work → recommend maintainer edit.
- Missing evidence → ask for minimal clarification.
- Duplicate → close with a pointer to the existing entry.
- Out of scope or unsafe → close politely.
- Premature or taxonomy-dependent → park.

Broken-link issues:

- Verify the link.
- Find a canonical replacement first; prefer official sources over mirrors.
- Remove only when no durable replacement exists.
- Leave a concise note explaining the action.

## Small Safe Fix Rule

When a resource is suitable and the issue is minor, make or recommend a maintainer edit rather than asking the contributor to revise.

Small safe fixes include: tightening a description, removing hype, fixing punctuation, correcting placement, replacing a non-canonical URL, matching bullet format, and removing tracking parameters.

## Stop and Ask

Stop before:

- Creating a new section or content file
- Reordering large parts of the README
- Editing the Contents block or scope-and-safety note
- Editing the Contributors section or badges
- Changing contribution rules or the safety boundary
- Removing several entries
- Making broad scope decisions
- Editing unrelated files

## Protected Areas

Do not edit unless explicitly instructed:

- The Contents block and section structure
- The intro and scope-and-safety note
- Badges
- The Contributors section and all-contributors markers
- Licence text
- Contribution and safety documents (`CONTRIBUTING.md`, `SECURITY.md`, `CODE_OF_CONDUCT.md`)
- Repository metadata unrelated to the task
- Private, local, draft, or scratch files

## Checks

There is no application build or test suite. After editing `README.md`, run or recommend the repository CI checks, which mirror the GitHub Actions workflows:

- `npx awesome-lint` — Awesome List linting (`.github/workflows/awesome-lint.yml`).
- Markdown link check — `.github/workflows/markdown-link-check.yml` uses `.github/mlc_config.json`; ignored or transient links are configured there.
- Repository health — `.github/workflows/repository-health.yml` confirms required files exist and that no forbidden content directories (`docs/`, `papers/`, `tools/`, `datasets/`, `benchmarks/`, `notes/`, `evaluation/`, `templates/`, `labs-and-companies/`) have been created.

## Maintainer Comment Templates

Accept: "Thank you — this is relevant, the link is canonical, and the placement works. I would accept this."

Maintainer edit: "Thank you — useful resource. I would accept it with a small maintainer edit to tighten the description and keep the wording neutral."

Request changes: "Thank you for the suggestion. I think this could fit, but I would ask for a little more context on why this is the canonical source and where it belongs."

Duplicate: "Thank you — I would close this as a duplicate because the resource already appears under [section]."

Out of scope: "Thank you for sharing this. I would close it because it sits outside the current scope of the list."

Park: "Thank you — this may be worth revisiting, but I would park it for now until the list has a clearer section for this category."

## Output Format

For PR or issue review, respond with:

- **Decision**: accept, maintainer edit, request changes, close, or park
- **Reason**: 1–3 bullets
- **Suggested README entry**, if useful
- **Suggested maintainer comment**
- **Files changed**, if any
- **Remaining uncertainty**, if any

## Editing Rule

Do not modify `README.md`, `CONTRIBUTING.md`, `SECURITY.md`, `.github` templates, or other files unless explicitly asked.
