# Architecture Decisions

## ADR-001: SOP execution is spec-driven

Task specs in `docs/specs/` are the default durable artifact between planning and implementation.

## ADR-002: Stable knowledge only goes to facts

`docs/facts/` stores only stable reusable context, not temporary task reasoning.

## ADR-003: Repeated workflows become skills

When a workflow is repeated and stable, it should be promoted into `skills/`.