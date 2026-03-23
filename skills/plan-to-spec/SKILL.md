---
name: plan-to-spec
description: Convert a plan, PRD, design note, or scoped request into one narrow executable task spec in docs/specs. Use when the user has direction but implementation should be narrowed before coding. Do not use when the task is already trivially narrow and spec-complete.
---

# Plan to Spec

## Purpose

Turn higher-level intent into a narrow, reviewable task spec.

## Inputs

- a plan
- a PRD
- a design note
- a scoped request
- an existing initiative slice

## Outputs

- one task spec in `docs/specs/YYYY-MM-DD-<task>.md`

## Steps

1. identify the smallest coherent implementation slice
2. define objective, scope, and non-goals
3. identify likely target files or systems
4. define validation at the spec level
5. keep the slice reviewable and narrow
6. write the spec using `docs/templates/task-spec-template.md`

## Guardrails

- do not generate a broad roadmap when one task spec is enough
- do not include speculative implementation detail
- do not omit non-goals
- do not create multiple specs unless the user asks or the work is clearly separable

## Trigger phrases

- turn this plan into an executable task
- derive a task spec
- make this implementation-ready
- convert this design into a coding task