# Instructions for agents using this playbook

This repository is a reusable **operating manual**, not the user's application repository. Follow it while creating/updating artifacts **in the target project's own repository**, unless explicitly asked to improve this playbook itself.

1. Read `docs/workflow.md` before taking action. Inspect actual target repository state; never assume a blank repo, that skills are installed, or that a past stage is complete.
2. Ask first: **"Do you already have a Product Overview, or should we create one together?"** If the answer is already evident in the repository or conversation, do not repeat the question. With an overview, assess it against `docs/product-overview-guide.md`; without one, use `templates/product-overview-v1.md` interactively.
3. Do only the **current checkpoint**. Ask essential decisions in the skill's intended format; wait for human approval before writing/finalizing major product artifacts or advancing through an approval gate.
4. Preserve the **product/technical boundary**. Product Overview and phased roadmap describe scope, behavior, limits, values, outcomes, dependencies and acceptance—not predetermined infrastructure, DB, frameworks, APIs or implementation.
5. For a prepared overview, ensure the target project and Matt skills are configured per `docs/matt-skills-setup.md` before running relevant skills. Read the **locally installed SKILL.md**; do not assume skill behavior from its name.
6. Use `$grill-me` specifically for **phased product roadmap discovery**; do not ask it to settle the whole product's technical architecture. Only finalize `docs/product/phased-roadmap-v1.md` after explicit approval.
7. Work through each approved phase independently, with its own bounded Wayfinder effort, then spec, tickets, execution and verification when those stages have been validated and are applicable. Do not claim untested steps are established practice.
8. **Minimal steering:** if an agent's recommendation is good, a short affirmative answer suffices (e.g. `Yes to all.`). Add corrective detail only when a proposal is wrong, materially ambiguous, or breaks a constraint. Do not inflate prompts with restatements of settled decisions.
9. Human decides consequential choices. Agent finds facts, reads files, proposes defaults with trade-offs, and reports status and evidence honestly. Never equate proposed/planned with done, passing tests with human acceptance, or a draft with approved.
10. Track the exact last approved checkpoint and provide a focused next action. Allow stopping and resuming without duplicating prior work.

**Do not auto-run the complete workflow after merely reading this document.** Begin by assessing the current checkpoint and request only the next necessary approval/action.
