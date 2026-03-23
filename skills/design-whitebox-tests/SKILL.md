---
name: design-whitebox-tests
description: Design proportional white-box validation for regression-sensitive or branch-heavy logic. Use when black-box checks alone are not enough to hold a fix or protect important internal behavior. Do not use for simple UI-only or trivial end-to-end changes.
---

# Design White-box Tests

## Purpose

Add focused white-box protection only when justified.

## Inputs

- a task spec
- changed code
- bugfix context
- regression risk

## Outputs

- recommended tests
- test targets
- justification for why white-box checks are needed

## Steps

1. identify the internal logic that is fragile or regression-sensitive
2. map important branches, state transitions, or contracts
3. propose the smallest set of tests that meaningfully protects behavior
4. avoid testing incidental implementation trivia
5. keep validation proportional to risk

## Guardrails

- black-box validation remains the default
- do not add coverage for coverage’s sake
- do not test private structure unless it protects meaningful behavior
- prefer deterministic regression tests for bugfixes

## Trigger phrases

- add regression protection
- design focused tests for this logic
- black-box checks are not enough
- add white-box validation