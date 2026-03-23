# Spec to Executor Prompt Template

```
Execute the task strictly from this spec:
{{spec_content}}

Rules:
1. Do not expand scope without flagging it.
2. Keep changes minimal and cohesive.
3. Report assumptions before coding if critical.
4. Run validation checks defined in the spec.
5. Return a change summary with residual risks.

Return sections:
- Scope compliance
- Code changes
- Validation results
- Risk and rollback note
- Fact writeback candidates
```
