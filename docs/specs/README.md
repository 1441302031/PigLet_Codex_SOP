# Specs README

Store one file per task in this directory.

## Lifecycle

1. Create file from `docs/templates/task-spec-template.md`.
2. Fill the required `Plan` and `Spec` sections.
3. Execute implementation against the spec.
4. Append validation results and change summary.
5. Add fact writeback only when the task produced a new durable, evidence-backed fact.

## Tips

- Keep assumptions explicit.
- Keep acceptance criteria observable.
- Keep risk mitigation actionable.
- Keep fact writeback limited to durable, evidence-backed knowledge.
- Use `N/A` when no stable fact was learned.
