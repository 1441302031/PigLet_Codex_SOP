# ai-engineering-sop-codex

Practical SOP for planning, specifying, implementing, validating, and documenting software changes with coding agents.

## Goal

Provide a repeatable workflow that keeps output stable across runs and across different agents.

## Standard Flow

1. Capture stable facts in `docs/facts/`.
2. Draft a plan with `docs/templates/plan-template.md`.
3. Convert plan to a task spec in `docs/specs/`.
4. Design whitebox tests before coding.
5. Implement in small safe changes.
6. Validate and summarize with `docs/templates/change-summary-template.md`.
7. Write back new facts to `docs/facts/`.

## Main Paths

- `docs/guides/`: process guides
- `docs/templates/`: reusable templates
- `docs/specs/`: task specs and execution artifacts
- `docs/facts/`: long-lived project knowledge
- `skills/`: task-oriented skill instructions
- `examples/`: sample end-to-end session

## Quick Start

1. Read `docs/guides/new-project-sop.md`.
2. Copy `docs/templates/task-spec-template.md` into `docs/specs/YYYY-MM-DD-task-name.md`.
3. Execute from the spec using the prompt templates.
4. Record validation and write back facts.
