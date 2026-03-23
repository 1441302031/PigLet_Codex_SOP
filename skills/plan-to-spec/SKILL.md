# Skill: plan-to-spec

## Purpose

Convert a rough implementation plan into a complete task spec.

## Inputs

- Raw plan notes
- Relevant facts from `docs/facts/`
- `docs/templates/task-spec-template.md`

## Steps

1. Extract objective and scope from the plan.
2. Identify assumptions and missing details.
3. Draft technical plan and acceptance criteria.
4. Define validation and rollback strategy.
5. Produce final spec in `docs/specs/`.

## Output

One completed spec file with all required sections.

## Quality Checks

- Scope is bounded.
- Acceptance criteria are testable.
- Validation commands are explicit.
