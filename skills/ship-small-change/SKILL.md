---
name: ship-small-change
description: Execute a task as the smallest coherent change with explicit validation and no unnecessary redesign. Use for normal implementation work after scope is already clear. Do not use for broad discovery or ambiguous product planning.
---

# Ship Small Change

## Purpose

Implement narrowly and finish with explicit validation.

## Inputs

- task spec
- existing scoped request
- target files

## Outputs

- minimal code or doc changes
- validation results
- optional write-back suggestions

## Steps

1. restate the scope boundary
2. identify the minimum file set to change
3. implement the smallest coherent change
4. run or describe explicit validation
5. report what changed and what did not
6. suggest fact write-back only if justified

## Guardrails

- no speculative refactors
- no opportunistic cleanup outside the slice
- no broad redesign
- no hidden scope expansion