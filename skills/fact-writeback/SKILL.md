# Skill: fact-writeback

## Purpose

Write newly validated project knowledge into durable fact documents.

## Inputs

- Task spec and change summary
- Validation evidence
- Existing files in `docs/facts/`

## Steps

1. Extract newly confirmed, stable information.
2. Reject speculative or temporary notes.
3. Update the relevant fact file.
4. Update `docs/facts/facts-index.md` if needed.

## Output

A concise fact update that future tasks can rely on.

## Quality Checks

- Every new fact has evidence.
- No task-specific transient details are stored as facts.
