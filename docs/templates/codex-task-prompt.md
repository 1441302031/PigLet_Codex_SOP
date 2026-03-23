# Codex Task Prompt Template

Read `AGENTS.md` and the relevant local `AGENTS.md` files first.

Then do the following:

1. summarize your understanding of the task and constraints
2. decide whether an existing spec can be reused
3. if needed, create a narrow task spec in `docs/specs/`
4. implement the smallest coherent change
5. validate explicitly
6. suggest stable fact write-back only if justified

Additional instructions:

- do not expand scope
- prefer black-box validation by default
- add white-box validation only when justified
- do not write temporary reasoning into `docs/facts/`
- use Chinese for user-visible summaries, progress updates, validation notes, and final output unless the task explicitly requires another language
