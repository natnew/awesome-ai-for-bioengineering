# AGENTS.md

Operating protocol for AI coding agents working in this repository.

Claude Code should read `CLAUDE.md` first, then use this file as the shared repository contract. Other agents should start here. Follow repository-local guidance over generic awesome-list assumptions.

## Repository North Star

This is a public, maintained Awesome List for AI engineering in bioengineering. The `README.md` is the product: a durable, high-signal, navigable map of the field for readers, contributors, and AI agents.

The list is curated, not accumulated. Each entry should help a reader understand the landscape, find a canonical resource, or compare related models, tools, datasets, and benchmarks. Selectivity, durability, clear placement, neutral description quality, and safety matter more than volume.

## Agent Role

Agents may help with:

- README maintenance when explicitly asked
- New entry review
- Pull request review
- Issue triage
- Broken-link checks
- Duplicate detection
- Section placement
- Description tightening
- Safety-boundary review
- Maintainer comment drafts
- Small, safe cleanup edits when explicitly requested

Agents must not:

- Add speculative or low-signal entries
- Inflate claims or preserve promotional wording
- Add any wet-lab, pathogen, genetic-manipulation, or synthesis detail
- Create content directories or category files outside `README.md`
- Reorganise the list or rewrite scope without explicit instruction
- Run broad formatting sweeps
- Edit unrelated files
- Touch protected areas unless explicitly instructed

## Read Order

Before reviewing or editing, read in this order:

1. `README.md` — scope, taxonomy, formatting, and existing examples
2. `CONTRIBUTING.md` — submission requirements and entry format
3. `SECURITY.md` — safety boundaries and out-of-scope content
4. `CLAUDE.md` — repository-specific rules for Claude and other agents
5. `.github/instructions/` — curation, link-quality, maintenance, and safety guidance
6. `.github/PULL_REQUEST_TEMPLATE.md` — contributor expectations
7. Recent issues and merged PRs, where available, for maintainer precedent

Do not assume the generic awesome-list pattern overrides this repository's existing structure.

## Repository Facts

- `README.md` is the primary and only content artefact. All curated resources live there.
- The README contains an intro, a scope-and-safety note, Contents, the main sections, Contributing, and Contributors.
- Sections are single-line bullet lists. Match the local format exactly.
- Entries take the form `* [Name](https://link) - Neutral, technically precise description.`
- Entries are kept in alphabetical order within a section where practical.
- One resource per pull request is preferred, with a short note on why it belongs.
- For code, prefer the official GitHub repository over a package registry or marketing page.
- For papers, prefer arXiv, DOI, or the official publisher or project page.
- New categories or structural changes are handled separately from single-entry contributions.

## Scope Rules

Belongs:

- Biological foundation models
- Protein language models
- Protein structure and function prediction
- Generative protein design
- Molecular generation and drug discovery
- DNA and RNA modelling
- Biomolecular simulation
- AI agents for science
- Self-driving laboratories and lab automation
- Synthetic biology tooling
- Datasets, benchmarks, and evaluation
- Reproducibility and validation resources
- Safety, security, and responsible release resources, at a governance level
- Academic labs, companies, platforms, and open-source tools in scope
- Durable surveys, papers, and technical explainers

Does not belong:

- Resources outside AI for bioengineering
- Thin wrapper pages or pure marketing pages
- Broken or inaccessible links
- Duplicate or near-duplicate resources
- Speculative or low-signal entries
- Unsupported ranking, performance, adoption, or novelty claims
- Time-sensitive claims such as "latest", "best", "leading", "fastest", or "most advanced"

## Safety Boundary (Hard Gate)

This is not a clinical, medical, laboratory, or experimental-protocol repository. The following must never enter the list, an entry description, an issue reply, or a PR comment:

- Wet-lab or experimental protocols
- Pathogen engineering or enhancement guidance
- Genetic-manipulation procedures
- Chemical or biological synthesis routes
- Any operational detail that could enable unsafe biological experimentation

Keep entries at the level of AI systems and what they model, predict, or generate. Responsible release and biosecurity resources are in scope at a high, governance-oriented level only. If a candidate drifts toward operational detail, generalise it or recommend declining. When in doubt, treat it as out of scope and flag the concern without restating the unsafe detail. See `SECURITY.md`.

## Quality Bar

An entry qualifies when all are true:

- It is clearly relevant to AI for bioengineering and fits an existing section.
- The source is canonical, credible, and useful to a technical reader.
- The link is durable, reachable, and uses HTTPS.
- The resource adds something distinct from existing entries.
- The description is neutral, concise, specific, and non-promotional.
- The entry contains no unsafe procedural detail.
- The formatting matches the surrounding section.
- No duplicate or stronger existing equivalent is already present.

## README Formatting Rules

- Preserve the existing heading and Contents structure.
- Preserve the intro, scope-and-safety note, Contributing, and Contributors sections.
- Add entries to the correct section in alphabetical order where practical.
- Use the single-line bullet format: `* [Name](https://link) - Description.`
- Use HTTPS and canonical links.
- Start descriptions with a capital letter and end with a full stop.
- Do not use title case for descriptions.
- Do not start descriptions with "A" or "An".
- Do not perform broad formatting changes unless explicitly asked.

## Link Quality Rules

Verify that:

- The link resolves and points to the canonical source.
- Repository links point to the main project, not an arbitrary fork.
- Paper links prefer arXiv, DOI, the publisher, or the project page.
- Dataset links prefer the official dataset page or a maintained repository.
- URLs do not include avoidable tracking parameters.
- Shortened and login-gated links are avoided.

## Description Style

Descriptions should be neutral, factual, specific, short, and free of hype or unsupported claims.

Prefer:

- "Diffusion model for generating protein backbones for design tasks."
- "Benchmark suite for de novo molecular design."
- "Curated database of bioactive molecules with drug-like properties."

Avoid:

- "Powerful", "revolutionary", "cutting-edge", "best", "latest", "industry-leading", "fastest"
- Unsupported claims about performance, adoption, or maturity

## Section Placement Rules

1. Identify the closest existing section in the Contents.
2. Compare the candidate with neighbouring entries.
3. Prefer the narrowest accurate section.
4. If two sections fit, choose the one where readers would most naturally look first.
5. Maintain alphabetical order within the section where practical.
6. Avoid creating a new section for a single item.
7. If placement is uncertain, state the trade-off and recommend one option.

## Duplicate Checking Rules

Before adding or approving, check for:

- Same URL
- Same project under a different URL
- Same paper title
- Same organisation and product name
- Renamed repositories
- An existing entry in a nearby section
- A stronger canonical source already listed

If a duplicate exists, recommend closing, editing, or redirecting rather than adding another entry.

## Decision Matrix

| Decision           | Use when                                                                                                  |
| ------------------ | --------------------------------------------------------------------------------------------------------- |
| Accept as-is       | In scope, canonical link, correct placement, matching format, neutral description, safe, no duplicate.    |
| Edit as maintainer | Strong resource needing small fixes: wording, punctuation, canonical URL, placement, or local formatting. |
| Request changes    | Resource may fit but evidence, link quality, relevance, or placement is materially unclear.               |
| Close              | Out of scope, duplicate, promotional, broken with no replacement, or no durable technical substance.      |
| Park               | Promising but immature, or requires maintainer judgement on taxonomy.                                     |

## Issue-to-Entry Workflow

For suggestion issues:

1. Check scope.
2. Check the safety boundary.
3. Check source and link quality.
4. Check duplicates.
5. Identify the best section.
6. Draft a neutral entry only if the resource qualifies.
7. Recommend accept, maintainer edit, request changes, close, or park.
8. Keep the maintainer comment concise.

For broken-link issues:

1. Verify the reported link.
2. Search for a canonical replacement.
3. Prefer official replacements over mirrors.
4. Preserve the entry if a durable replacement exists.
5. Recommend removal only when no credible replacement exists.

## Pull Request Review Workflow

1. Read the PR title, description, and diff.
2. Confirm it changes only `README.md` (or the relevant support file) and nothing unrelated.
3. Check each added or changed link.
4. Check scope, source quality, and the safety boundary.
5. Check duplicates and section placement.
6. Check local formatting and alphabetical order.
7. Neutralise description language where needed.
8. Decide: accept, maintainer edit, request changes, close, or park.
9. Draft a concise maintainer comment.

Minimise contributor friction. If the resource is clearly suitable and the issue is minor, recommend a maintainer edit rather than asking the contributor to revise.

## Verification Checks

After editing `README.md`, run or recommend the repository CI checks:

- awesome-lint
- link check
- repository-health

## Stop and Ask

Stop and ask the maintainer before:

- Creating a new section or content file
- Reordering large parts of the README
- Changing the Contents structure
- Changing contribution rules or safety boundaries
- Removing multiple entries
- Making judgement-heavy scope changes
- Editing files unrelated to the stated task

## Protected Areas

Do not edit unless explicitly instructed:

- The Contents block and section structure
- The intro and scope-and-safety note
- The Contributors section and all-contributors markers
- Badges
- Licence text
- Contribution and safety documents (`CONTRIBUTING.md`, `SECURITY.md`, `CODE_OF_CONDUCT.md`)
- Private, local, draft, or scratch files

## Maintainer Comment Style

Comments should be warm, concise, respectful, and decision-oriented.

Prefer:

- "Thank you for the suggestion. This is relevant, the link is canonical, and I would place it under X with a shorter neutral description."
- "Thank you — useful resource. I would accept this with a small maintainer edit to remove the ranking claim."
- "Thank you for raising this. I would close it as a duplicate because the resource already appears under X."
- "Thank you — I would park this until the list has a clearer section for this category."

Avoid long explanations, harsh rejection wording, defensive language, and asking contributors for trivial edits the maintainer can safely make.

## Final Response Pattern

When finishing a task, summarise:

- What was reviewed
- Decision or recommended decision
- What changed, if anything
- Any safety or link-quality risks or uncertainties
- Suggested maintainer comment, if relevant
- Follow-up needed, if any

Do not modify `README.md` or other files unless explicitly asked.
