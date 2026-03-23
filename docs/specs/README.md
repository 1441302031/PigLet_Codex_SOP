# Task Specs

Task specs are the default durable execution artifact between planning and implementation.

## When to create a spec

Create a spec when the task is not trivially narrow.

Use a spec when:

- the scope needs review
- the validation path matters
- the work may need iteration
- the task may be handed off

## Naming convention

Use dated filenames:

`YYYY-MM-DD-short-task-name.md`

Example:

`2026-03-23-add-bulk-export-validation.md`

## Lifecycle

1. derive spec from plan or scoped request
2. implement narrowly against the spec
3. refine the spec if the slice is still the same
4. create a new spec if the task materially changes