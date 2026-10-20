# Human–agent collaboration and prompting

## Working agreement (observed)

**Human:** owns vision, scope decisions, approvals, credentials, repository creation/clone and decisions delegated to them.

**Coding agent:** inspects the repository, reads actual installed skills, finds facts, asks only necessary decisions, documents approved outputs, and later builds/tests within the currently authorized scope.

**Advisor/reviewer:** evaluates the agent's questions and recommendations and helps produce only the needed response.

## Minimal steering rule

- **Agree with recommendation:** reply `Yes.`, `Yes to all.`, or the stated option. Do not rephrase the same decision into a long steering prompt.
- **Disagree:** briefly explain *what is wrong* and provide a narrow correction respecting prior decisions.
- **Important ambiguity:** clarify that ambiguity only.
- **Next frontier:** let the installed skill decide the next questions; do not add side quests.
- **Approval:** a short `Yes, this captures our shared understanding. Proceed.` is sufficient at a required final alignment check.

### Concrete reference

During Repository-to-Course roadmap discovery, Codex presented Q1–Q4, Q5–Q8, and Q9–Q12, each with recommended `yes` answers. The human accepted these rounds with `Yes to all.` The final six-phase structure was separately approved before Codex wrote its file.

This is **not** a recommendation to accept every agent proposal. Audit for conflicts first; avoid needless elaboration **when the recommendation is already correct**.

## Prompt discipline

1. State one skill, one purpose, one primary reference, and one expected deliverable.
2. Keep current task at the proper decision layer (product vs technical).
3. Name exclusion of premature work *only when the boundary needs protection*.
4. Prefer reading existing decisions to repeating them in the next prompt.
5. Agent questions and review happen round by round, not as a huge one-shot instruction dump.

## No invented progress

Use clear statuses: proposed, approved, documented, implemented, verified, released. Read the actual repo before describing a step as complete.
