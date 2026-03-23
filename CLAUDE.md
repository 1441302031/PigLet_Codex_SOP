# Claude Collaboration Guide

Use this file as a model-specific operating brief.

## Expected Behavior

- Read `docs/facts/facts-index.md` before planning.
- Use templates from `docs/templates/` instead of free-form structure.
- Keep diffs small and include validation notes.
- Record assumptions explicitly.

## Output Format

When handling a task, follow this order:

1. Problem framing
2. Plan
3. Spec
4. Implementation notes
5. Validation evidence
6. Change summary
7. Fact writeback

## Escalation

Escalate when:

- Scope expands beyond the original task.
- Hidden dependencies or migrations appear.
- Validation is blocked by environment limits.
