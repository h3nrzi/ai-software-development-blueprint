# Operating workflow — v0.1

**Purpose:** enable an agent to guide a human through an entire software-product lifecycle with explicit checkpoints, reusable templates, and no premature technical commitments.

## Startup / resume protocol

1. Identify the **target project repository** (do not confuse it with this blueprint). Look for existing product documents, agent instructions, installed skills, plans, changes and recorded approvals.
2. Report in a few lines: **known current checkpoint, evidence, missing prerequisite, one next action**. Never overwrite existing artifacts without checking.
3. Start at the **earliest incomplete gate** below. If the user already provided the necessary answer, continue without re-asking.
4. Perform only that gate. Save agreed outputs in the target repository, verify the actual files, report progress, and await the next instruction where human approval is needed.
5. Later gates remain provisional until tested in a real project and incorporated here with evidence.

## Gate 1 — Product Overview

**First question (when unanswered):** "Do you have a Product Overview already, or would you like us to build one together?"

- **Exists:** locate and read the full overview; use `docs/product-overview-guide.md` to check coverage, contradictions and unknowns. Do not force a rewrite when it is good enough.
- **Missing:** use `templates/product-overview-v1.md` as the adaptable scaffold; explore the idea conversationally, with meaningful questions and recommended defaults.
- **Output:** `docs/product/product-overview-v1.md` in the target repo (unless its existing convention says otherwise).
- **Gate:** human approves the product-level description and V1 boundaries. No tech stack or implementation architecture selected here.

## Gate 2 — Project and skills readiness

- Verify target GitHub repository, local working copy if applicable, and the agent environment.
- In the reference project, the human cloned the repository and ran `$setup-matt-pocock-skills` in Codex. See `docs/matt-skills-setup.md`.
- Inspect target `AGENTS.md`, skill installation, tracker convention and domain-doc guidance; use the real local skill instructions.
- If already configured, skip setup instead of redoing it.
- **Gate:** the agent can identify which skills are installed, where issues/specs live, and which conventions govern work.

This readiness gate may happen **before or during** the Product Overview stage if needed. The reference project's setup occurred before its roadmap discussion; do not impose a fictional universal order.

## Gate 3 — Phased Product Roadmap (validated discovery workflow)

- Input: complete approved overview + repo guidance.
- Skill: `$grill-me` (the installed `grilling` behavior was observed asking a whole ready decision frontier per round).
- Discuss coherent **product-oriented vertical phases**, their scope allocations, dependencies, user-visible outcomes and completion gates.
- Use recommendations and trade-offs; user may approve an entire sound round with `Yes to all.`
- Coverage: every committed V1 capability appears in the roadmap; future ideas remain explicitly future.
- Do **not** resolve all technical questions for the entire product; Wayfinder will handle phase-local uncertainty.
- Present the full proposed sequence, obtain explicit human approval **before** writing/finalizing it.
- **Output:** `docs/product/phased-roadmap-v1.md`.
- **Gate:** each phase has goal/outcome, in-scope, out-of-scope, dependencies, product acceptance, completion conditions, and focused Wayfinder handoff.
- A single six-phase roadmap was right for Repository-to-Course; **other projects may need a different number**.

## Gate 4 — Phase-by-phase delivery (planned, not yet experience-validated)

For the **next approved incomplete phase** only:

```text
Read Product Overview + full roadmap + current phase
  → $wayfinder: phase-local decision map and resolution
  → $to-spec: bounded specification
  → $to-tickets: executable work units
  → $implement / $implement-spec as appropriate
  → review, test, human acceptance, record phase completion
  → next phase
```

Treat each skill as its own process, read its local instructions, and respect its stopping conditions. Wayfinder is planning by default and **does not mean "implement"**. Do not turn product-roadmap phases into fixed technical architectures.

**Unvalidated specifics:** exact implementation/review/release mechanics and issue tracker integration will be refined with actual experience. This is a navigation scaffold, not a claim they are already proven.

## Gate 5 — Product release (planned)

Verify product-specific acceptance, quality checks, operational readiness and explicit release approval. Actual process to be documented from future experience.

## Universal stop conditions

Stop and seek human input when:
- a consequential product boundary is undecided;
- skill installation or a required file cannot be verified;
- a completed checkpoint appears inconsistent or needs replacement;
- human sign-off is required and has not been given;
- scope grows beyond the selected phase.

Avoid giant prompts, speculative configuration and generating the entire set of future artifacts at once.
