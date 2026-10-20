# Evidence, maturity, and next-learning checkpoints

**As of 2026-10-20.** This file deliberately distinguishes observed working practice from an intended future flow. Do not mark a checkpoint proven merely because it is documented.

| Checkpoint | State | Grounding |
| --- | --- | --- |
| Target repository creation and skills setup | Observed | [Repository-to-Course setup commit](https://github.com/h3nrzi/Repository-to-Course/commit/fc6cd4c1b201896767f65b80ad50df8a633b86a7), Codex setup transcript |
| Comprehensive Product Overview available | Observed | [V1 overview](https://github.com/h3nrzi/Repository-to-Course/blob/main/docs/product/product-overview-v1.md) |
| Interactive creation of a Product Overview using **this** generalized template | **Not yet tested** | Template abstracted from existing approved document; needs a new-project trial |
| grill-me scoped to phased Product Roadmap | Observed | 12 approved questions in 3 rounds, final alignment, [roadmap](https://github.com/h3nrzi/Repository-to-Course/blob/main/docs/product/phased-roadmap-v1.md) |
| Independent Wayfinder session for a selected phase | **Pending** | Next planned experiential checkpoint |
| to-spec and to-tickets after that Wayfinder | **Pending** | Not part of observed run |
| Ticket-by-ticket implementation/review with the project | **Pending** | Not yet demonstrated in the reference |
| Release, handoff, repeatable resume/recovery | **Pending** | Need real usage evidence |

## Case study: Repository-to-Course

Source repository: https://github.com/h3nrzi/Repository-to-Course

Observed path:

1. User created/cloned project and configured AI Hero skills through Codex.
2. Established local Markdown issue tracking, domain-doc guidance and agent instructions.
3. Created comprehensive Product Overview (22 sections, V1 boundaries and future vision).
4. Scoped `grill-me` to **phased Product Roadmap discovery** rather than whole-product technical design.
5. Three decision frontiers: Q1–4, Q5–8, Q9–12. Human accepted recommended decisions, with concise `Yes to all.`.
6. Agent presented six-phase structure. Human explicitly approved.
7. Codex wrote `docs/product/phased-roadmap-v1.md`, covering phase goals, capabilities, boundaries, dependencies, product acceptance, completion, and phase-local Wayfinder handoffs.
8. Product Overview and roadmap were committed on `main`: [2f08e51](https://github.com/h3nrzi/Repository-to-Course/commit/2f08e51d913f5df194236f8f88cebd593ecc5528).

### Distilled lessons

- The overview is an authoritative **product** reference, not an architecture specification.
- A project can be too large for a single unconstrained Wayfinder. First agree on product-sized phases.
- Matt's grilling asks questions in a decision frontier; do not force an unrelated single-question pattern on that skill.
- Minimal steering: agree succinctly when the recommendation is sound; elaborate only to correct.
- Human sign-off is a real gate. Written planning alone is not implementation, acceptance or validation.
- Keep the generalized playbook distinct from source-project-specific V1 policies, content and constraints.

## Maintenance rule

After each real experience in Repository-to-Course:
1. Link to the source commit/artifact and record what happened.
2. Distinguish approved decision, agent proposal, and verified outcome.
3. Update only the relevant playbook step and its recovery/approval rule.
4. Avoid making new projects inherit domain-specific decisions from the example.
5. Retest agent instructions from a fresh target project when the flow changes.

**Next experience to incorporate:** the selected phase's actual Wayfinder session. Do not fabricate its findings now.
