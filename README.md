# AI Software Development Blueprint

An **agent-readable, human-led playbook** for guiding a software product from the first idea through release using coding agents and Matt Pocock's skills.

> **Current maturity:** Discovery and phased-roadmap workflow documented from a real project. Technical discovery, specification, ticketing, implementation, testing, and release procedures are **not yet validated in this playbook**. Do not pretend otherwise.

## Start here

**For a human:** Ask your coding agent to read [AGENTS.md](AGENTS.md), then follow [the operating workflow](docs/workflow.md) **one step at a time**. Keep your own project repository as the location of its product artifacts and implementation.

**For an agent:** Read `AGENTS.md` and `docs/workflow.md`. Inspect the target project, find the first incomplete checkpoint, ask only the next necessary question, and stop at human-approval gates. Do not jump ahead or produce all documents in one pass.

## Core flow

```text
Check whether Product Overview exists
  ├─ yes → review it against the standard and resolve only important gaps
  └─ no  → collaboratively create it from the template
          ↓ creator approval
Prepare / verify target repository and Matt skills
          ↓
Run grill-me for PRODUCT ROADMAP DISCOVERY
          ↓ creator approval
Save a phased product roadmap
          ↓
For each approved phase:
    wayfinder → to-spec → to-tickets → implement → validation/review
          ↓
    complete the phase only when its evidence and approvals justify it
          ↓
Product release
```

The later skill chain is an **intended workflow**, not evidence that those steps have been completed in the reference project.

## Documents

- [Agent operating rules](AGENTS.md)
- [Step-by-step workflow and resume rules](docs/workflow.md)
- [Product Overview template](templates/product-overview-v1.md)
- [Product Overview quality gate](docs/product-overview-guide.md)
- [Roadmap discovery and handoff](docs/roadmap-discovery.md)
- [Skill setup notes](docs/matt-skills-setup.md)
- [Minimal steering and human approvals](docs/agent-collaboration.md)
- [Evidence log and open gaps](docs/evidence-and-status.md)

## Provenance

This playbook records lessons learned from [Repository-to-Course](https://github.com/h3nrzi/Repository-to-Course), specifically its [Product Overview](https://github.com/h3nrzi/Repository-to-Course/blob/main/docs/product/product-overview-v1.md), [approved phased roadmap](https://github.com/h3nrzi/Repository-to-Course/blob/main/docs/product/phased-roadmap-v1.md), and the human/Codex discussion that produced them.

The **22-section overview is a reference example, not a mandatory 22-section format for every product**. Product decisions specific to Repository-to-Course must not be imported into unrelated projects.
