# New Project SOP

This guide defines the default execution process for a new task or project slice.

## Stage 0: Intake

- Capture request, objective, constraints, and success signal.
- Confirm out-of-scope boundaries.

## Stage 1: Facts

- Read `docs/facts/facts-index.md`.
- Update or create facts only when evidence is clear.
- Avoid speculative facts.

## Stage 2: Plan

- Use `docs/templates/plan-template.md`.
- Split work into small, testable increments.
- Flag unknowns and risks early.

## Stage 3: Spec

- Use `docs/templates/task-spec-template.md`.
- Define acceptance criteria and validation method.
- Include rollback strategy for risky changes.

## Stage 4: Test Design

- Design whitebox tests from expected code paths.
- Include one happy path and one failure path minimum.

## Stage 5: Implementation

- Ship in small commits or logical steps.
- Keep behavior changes traceable to spec criteria.

## Stage 6: Validation and Summary

- Run checks listed in `docs/facts/validation-policy.md`.
- Summarize using `docs/templates/change-summary-template.md`.

## Stage 7: Fact Writeback

- Record newly confirmed knowledge.
- Update `docs/facts/facts-index.md` with links.
