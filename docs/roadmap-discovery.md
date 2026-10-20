# Product roadmap discovery with grill-me

**Validated reference:** [Repository-to-Course phased roadmap](https://github.com/h3nrzi/Repository-to-Course/blob/main/docs/product/phased-roadmap-v1.md).

## Preconditions

- Read approved `docs/product/product-overview-v1.md` in full, not just an executive summary.
- Inspect target repo guidance and installed skills.
- Ensure that "V1" and "later" product boundaries are explicit.

## Give the skill the right destination

Use `$grill-me` to build a **phased product development roadmap**, not a complete technical specification.

The roadmap splits all committed V1 behaviors into progressive learner/user-visible increments, each with product scope and explicit completion gates. It should not invent the framework, database, APIs, deployment architecture or technical decisions.

## Interaction observed

- Grill asks the whole *ready frontier* of questions in rounds, each numbered and with recommended yes-able answers.
- The user approves or corrects each round.
- Codex restates a proposed six-phase roadmap and seeks final confirmation.
- Only then does it create `docs/product/phased-roadmap-v1.md`.
- The result retains the overview as primary authority and includes common safeguards, phase definitions, V1 coverage, future exclusions and Wayfinder handoffs.

## Required phase schema

For each phase:
1. Goal and user-visible outcome.
2. In-scope capabilities and behaviors.
3. Explicit out-of-scope.
4. Dependencies on earlier phases.
5. Product-level acceptance criteria.
6. Clear completion conditions.
7. Focused handoff for an **independent** Wayfinder effort.

Avoid technical-layer phases such as "database → API → UI", and avoid prematurely turning a roadmap into tickets.

## Why this boundary matters

`$grill-me` resolves **roadmap shape and scope allocation**. `$wayfinder` later resolves **specific unresolved decisions for one phase**. Feeding the complete product to a single Wayfinder can create an excessively wide planning map; splitting first keeps decisions bounded.

## Example of a short task request

```text
Use $grill-me for PRODUCT ROADMAP DISCOVERY.
Primary reference: docs/product/product-overview-v1.md
Deliverable: docs/product/phased-roadmap-v1.md
Ask about phase boundaries, sequencing, dependencies, scope and acceptance.
Do not decide implementation architecture.
Present the roadmap for explicit approval before writing it.
```

Use this as **an example**, not a reason to add more steering than the agent needs.
