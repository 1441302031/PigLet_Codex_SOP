# Agent Operating Notes

This repository is optimized for coding-agent collaboration.

## Core Principles

- Safety first: prefer small, reversible changes.
- Facts over assumptions: check `docs/facts/` before planning.
- Spec before code: every non-trivial change needs a task spec.
- Validation is required: implementation is not done without checks.
- Writeback is required: update durable knowledge after each task.

## Task Contract

For each task, produce:

1. A plan section.
2. A spec section.
3. A validation section.
4. A change summary section.
5. A fact writeback section when new knowledge appears.

## Definition of Done

- Behavior change is implemented.
- Validation evidence is captured.
- Risks and follow-ups are listed.
- Relevant facts are updated.
