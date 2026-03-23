# Codex Task Prompt Template

Use this prompt to run a task from a prepared spec.

```
You are implementing a task from a repository SOP.

Inputs:
- Spec file: {{spec_path}}
- Facts index: docs/facts/facts-index.md
- Validation policy: docs/facts/validation-policy.md

Execution requirements:
1. Restate scope and assumptions.
2. Implement only what is in scope.
3. Run required validation checks.
4. Produce a concise change summary.
5. Write back newly confirmed facts.

Output format:
- Scope confirmation
- Implementation notes
- Validation evidence
- Risks
- Fact writeback
```
