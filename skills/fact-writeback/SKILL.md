---
name: fact-writeback
description: Decide whether information from a task should be written back into docs/facts and place it in the right fact file. Use when stable reusable context emerged from execution. Do not use for temporary notes, debugging chatter, or task-local reasoning.
---

# Fact Write-back

## Purpose

Write back only stable reusable project context.

## Inputs

- implementation outcome
- validation outcome
- stable scope clarification
- durable workflow or architecture decision

## Outputs

- proposed fact updates in `docs/facts/*`
- no-op when write-back is not justified

## Decision rule

Write back only if the information is:

- stable
- reusable
- worth re-reading later

## Steps

1. identify candidate facts
2. reject temporary or local-only reasoning
3. map each valid fact to the right file
4. keep fact wording concise and durable
5. avoid duplicating rules already captured elsewhere

## Guardrails

Never write back:

- temporary debugging notes
- one-off implementation details
- unstable exploration
- conversational residue