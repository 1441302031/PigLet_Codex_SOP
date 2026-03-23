# AGENTS.md

## Purpose

This repository is a Codex-ready SOP for AI-assisted engineering.

The operating model is:

- plan-first engineering
- task-spec-driven execution
- smallest coherent implementation
- explicit validation
- stable fact write-back
- skill promotion for repeated workflows

## Default execution sequence

Follow this sequence by default:

1. understand the request and project constraints
2. decide whether a durable plan is needed
3. create or refine one narrow task spec in `docs/specs/` unless the task is trivially narrow
4. implement the smallest coherent change
5. validate explicitly
6. propose stable fact write-back only when justified
7. promote repeated workflows into skills only when they are stable and reusable

Default path:

`plan -> spec -> implementation -> validation -> fact write-back`

## What to read first

When starting work in this repository:

1. read this file
2. read `docs/specs/README.md`
3. read `docs/facts/project-scope.md` if it exists
4. check whether the task already has an existing spec in `docs/specs/`

## Scope control

- prefer the smallest coherent change
- do not widen scope without clear instruction
- do not redesign the system because a broader rewrite looks cleaner
- do not create speculative abstractions
- do not convert temporary reasoning into permanent documentation

## Spec rule

Create a task spec when:

- the task spans multiple edits
- the validation path needs to be explicit
- the work should be reviewable or handoff-friendly
- the scope boundary matters

A spec may be skipped only for trivially narrow, already well-scoped tasks.

If a task changes meaningfully, create a new dated spec instead of silently mutating the old one.

## Validation rule

Black-box validation is the default.

Add white-box validation when logic is:

- branch-heavy
- regression-sensitive
- stateful
- internally fragile
- protected by important contracts

Validation must be concrete and reviewable.

## Fact write-back rule

Only write back information that is:

- stable
- reusable
- worth re-reading later

Write stable facts to `docs/facts/*`.

Do not write back:

- temporary debugging notes
- one-off implementation chatter
- unstable exploration
- task-local reasoning with no future reuse value

Before writing back, ask:

1. will this still matter later?
2. can it be reused later?
3. is there a clear destination file?

If not clearly yes, do not write it back.

## Skill usage rule

Use a skill when a workflow repeats and has recognizable inputs and outputs.

Do not create a new skill for every one-off prompt.

## Output expectations

When working on a task, prefer this output order:

1. summary of understanding
2. plan or reference to existing spec
3. proposed file changes
4. implementation
5. validation results
6. optional fact write-back suggestions

## Editing expectations

When changing this repository itself:

- keep changes narrow
- keep terminology consistent
- update the right layer instead of duplicating rules
- prefer refinement over expansion