# Design to Spec Handoff

Use this handoff when turning product/design input into an engineering spec.

## Inputs Required

- Business goal and non-goals
- User flow and edge cases
- Constraints (performance, security, compliance, timeline)
- Existing system dependencies

## Handoff Checklist

1. Scope is explicit and bounded.
2. Terminology is consistent.
3. Open questions are listed.
4. Unknowns are marked as assumptions.
5. Acceptance criteria are testable.
6. Monitoring and rollback are considered.

## Output Contract

Generate one spec file in `docs/specs/` containing:

- Context
- Scope and non-scope
- Technical approach
- Test plan
- Rollout and rollback plan
- Risks and mitigations

## Quality Gate

A handoff is complete only if another engineer can implement without synchronous clarification.
