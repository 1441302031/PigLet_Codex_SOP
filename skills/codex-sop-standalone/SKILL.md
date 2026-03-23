---
name: codex-sop-standalone
description: Standalone Codex SOP workflow for local projects. Use when Codex needs one directly invocable skill to handle spec creation, scoped task execution, regression-sensitive test planning, and fact write-back decisions without depending on other repository skills.
---

# Codex SOP Standalone

## Purpose

Provide one self-contained skill that can be copied into another local project and invoked as `$codex-sop-standalone`.

Use it to run a small, consistent SOP:

- read local rules first
- create or refine one narrow spec when needed
- implement the smallest coherent change
- validate explicitly
- suggest fact write-back only when justified

## Use This Skill When

- the local project wants one installable SOP skill instead of several smaller skills
- the task may involve `spec`, `task`, `test`, or `facts`
- the project needs a spec-first workflow without copying instructions from this repository by hand
- the user wants a direct `$codex-sop-standalone` entry point

## Do Not Use This Skill When

- the task is a one-line request that does not need SOP structure
- the project already has a different mandatory workflow that this skill would conflict with
- the user only needs one highly specialized sub-workflow and not an end-to-end SOP

## Inputs

- user request
- local project files
- local project rules such as `AGENTS.md`
- existing `docs/specs/`, `docs/facts/`, and validation commands when present

## Outputs

- one narrow next step
- a spec when the task is not trivially narrow
- minimal implementation guidance or execution
- explicit validation results
- optional fact write-back suggestion only when clearly justified

## Workflow

### 1. Read local rules first

- Read the nearest `AGENTS.md` first.
- If the project has additional local operating rules, follow them before this skill's defaults.
- If no local rules exist, use the default path:

`plan -> spec -> implementation -> validation -> fact write-back`

### 2. Handle `spec`

- Create a dated spec in `docs/specs/` when the task spans multiple edits, needs explicit validation, or needs clean scope boundaries.
- Keep the spec narrow.
- Always define:
  - objective
  - scope
  - non-goals
  - target files or areas when known
  - validation plan
  - completion criteria

### 3. Handle `task`

- Implement the smallest coherent change.
- Do not widen scope without explicit instruction.
- Do not refactor unrelated code.
- Prefer refinement over expansion.

### 4. Handle `test`

- Prefer black-box validation by default.
- Add white-box checks only when black-box testing is insufficient for branch-heavy, stateful, fragile, or regression-sensitive logic.
- Design the smallest regression-sensitive test set that proves the changed behavior and guards the most likely regressions.
- Validation must be concrete and reviewable.

### 5. Handle `facts`

- Suggest fact write-back only if the information is stable, reusable, and worth re-reading later.
- Do not write back:
  - temporary debugging notes
  - unstable exploration
  - one-off implementation chatter
  - task-local reasoning with no future reuse value

### 6. Language rule

- Use Chinese for user-visible output unless the user explicitly requests another language.
- Keep code, commands, paths, identifiers, and quoted literals in the form most useful for execution and review.

## Minimal Invocation Examples

- `Use $codex-sop-standalone to turn this request into a narrow spec.`
- `Use $codex-sop-standalone to implement the smallest coherent change from this spec.`
- `Use $codex-sop-standalone to design the smallest regression-sensitive test set for this change.`
- `Use $codex-sop-standalone to decide whether this task justifies stable fact write-back.`

## Installation

Copy the entire `codex-sop-standalone/` folder into another local project's skills directory.

This skill is designed to remain usable even if the target project does not copy this repository's other skill folders.

## Guardrails

- keep scope narrow
- do not require other skills as hard dependencies
- do not silently create broad roadmaps when one narrow task spec is enough
- do not recommend fact write-back without durable evidence
