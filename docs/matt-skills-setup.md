# Matt Pocock skills: setup observations

## Observed in Repository-to-Course

- A GitHub project repository was created and cloned by the human.
- The human installed/setup Matt Pocock's AI Hero skills using `$setup-matt-pocock-skills` in Codex.
- Codex added root `AGENTS.md` and `docs/agents/issue-tracker.md`, `docs/agents/triage-labels.md`, `docs/agents/domain.md`.
- The human chose **Local Markdown** as the issue tracker. The observed convention was `.scratch/<feature-slug>/spec.md` with numbered work items under `.scratch/<feature-slug>/issues/`.
- Domain documentation convention: root `GLOSSARY.md` and architecture records under `docs/adr/` (created lazily when needed).
- Skills were present under `.agents/skills/` with skill installation tracked by `skills-lock.json`.
- Reference project setup commit: [fc6cd4c](https://github.com/h3nrzi/Repository-to-Course/commit/fc6cd4c1b201896767f65b80ad50df8a633b86a7).

## How to guide another project

1. **Inspect before installing.** Check the target repo for skill files and instructions, tracker selection, and any pre-existing agent setup.
2. If absent, have the human run the actual setup skill in their Codex environment. Read its current local instructions and follow its prompts.
3. Let the human decide tracker and documentation conventions. Do not silently force Local Markdown as universal.
4. Confirm the written configuration and available skill names from the project itself. Do not invent commands or assume Matt skills have fixed semantics across revisions.
5. Resume the product workflow from the latest approved checkpoint.

**Important:** This blueprint documents Matt skills but does **not** vendor or redistribute their source code. The target project is responsible for installing and locking its selected skills.

## Skills relevant to the present journey

- `setup-matt-pocock-skills`: setup (observed)
- `grill-me` / installed grilling skill: product-roadmap questions, when explicitly scoped (observed)
- `wayfinder`: bounded, phase-local decision planning (read/observed guidance; phase usage pending)
- `to-spec`, `to-tickets`, `implement`: intended later chain (not yet completed in this case study)

Do not confuse roadmap discovery with Wayfinder's ticket-level decision discovery.
