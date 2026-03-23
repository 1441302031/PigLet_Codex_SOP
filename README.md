# AI Engineering SOP for Codex

A Codex-ready SOP repository for AI-assisted engineering.

This repository turns a lightweight AI engineering SOP into a Codex-usable operating system for daily work. It is designed for plan-first engineering, narrow task execution, explicit validation, stable fact write-back, and reusable skills.

## What this repository is for

Use this repository when you want Codex to work with a consistent engineering workflow:

1. understand the project rules from `AGENTS.md`
2. start from a plan or scoped request
3. derive one narrow task spec in `docs/specs/`
4. implement the smallest coherent change
5. validate explicitly
6. write back only stable reusable facts
7. promote repeated workflows into `skills/`

## Core workflow

The default path is:

`plan -> task spec -> implementation -> validation -> fact write-back -> skill promotion`

## How Codex should use this repo

- Read `AGENTS.md` first.
- Use `docs/templates/task-spec-template.md` when a task needs a durable execution artifact.
- Use `skills/plan-to-spec/` when the user gives a plan, PRD, or design and needs an executable task spec.
- Use `skills/design-whitebox-tests/` when black-box checks are insufficient.
- Use `skills/fact-writeback/` to decide what stable context belongs in `docs/facts/`.
- Prefer the smallest coherent change.

## Minimal startup

1. Open Codex in the repository root.
2. Ask Codex to read `AGENTS.md`.
3. Give it a task:
   - “Create a plan and derive a task spec for adding X.”
   - “Use the existing spec in docs/specs and implement the smallest coherent change.”
4. Review validation output.
5. Write back only stable facts.

## Recommended task prompt

See `docs/templates/codex-task-prompt.md`.

## Repository layout

- `AGENTS.md` canonical working rules
- `.codex/config.toml` Codex project settings
- `docs/specs/*` task execution artifacts
- `docs/templates/*` reusable templates
- `docs/facts/*` stable project context
- `skills/*` Codex skills for recurring workflows

## Adoption notes

This repository keeps the SOP tool-neutral in spirit, but it is structured so Codex can directly consume project instructions and reusable skills.