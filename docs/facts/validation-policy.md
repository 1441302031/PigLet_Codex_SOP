# Validation Policy

## Default

Black-box validation is the default acceptance mechanism.

## Add white-box validation when

- logic is branch-heavy
- regressions are likely
- internal contracts matter
- stateful behavior is fragile
- a bugfix needs deterministic protection

## Rule

Validation must be concrete, reviewable, and proportional to the task.