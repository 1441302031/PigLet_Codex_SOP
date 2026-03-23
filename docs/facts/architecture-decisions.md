# Architecture Decisions

## ADR-001: Spec-First Workflow

- Status: accepted
- Context: ad hoc coding leads to drift and unclear acceptance.
- Decision: require written task spec before non-trivial implementation.
- Consequence: slightly higher upfront effort, much clearer execution.

## ADR-002: Fact Writeback

- Status: accepted
- Context: repeated rediscovery slows delivery.
- Decision: write back stable findings into facts docs.
- Consequence: lower future onboarding and investigation cost.

## ADR-003: Small Safe Changes

- Status: accepted
- Context: large diffs increase risk and review load.
- Decision: ship minimal cohesive changes with explicit validation.
- Consequence: faster feedback loops and safer rollback.
