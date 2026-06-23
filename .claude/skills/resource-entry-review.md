# Skill: resource-entry-review

Evaluate a proposed `README.md` entry before it is added.

## Inputs

- Proposed name, URL, target section, and description.

## Steps

1. **Relevance** — Is it directly relevant to AI engineering for bioengineering? If not, reject.
2. **Signal** — Is it technically meaningful and durable, not marketing-led or thin?
3. **Source** — Is the URL the canonical home (repository, paper, documentation, project page) and HTTPS? Fix or reject if not.
4. **Placement** — Is the target section correct? Suggest the right one if not.
5. **Duplicate** — Does an equivalent entry already exist? If so, reject or merge.
6. **Description** — Rewrite to one neutral line: what the system is and what it models, predicts, or generates. Remove hype.
7. **Safety** — Confirm no unsafe biological procedural detail. Generalise or reject if present.

## Output

- Decision: accept / revise / reject, with a one-line reason.
- If accept or revise, the final entry: `- [Name](https://link) - Description.`
