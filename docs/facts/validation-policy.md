# Validation Policy

All behavior changes require validation evidence.

## Required Checks

1. Static checks (lint/type/format) when available.
2. Unit or integration tests for affected paths.
3. Manual verification for UX or workflow changes.

## Evidence Standard

- Record command used.
- Record high-level result.
- Record known gaps when checks cannot run.

## Failure Handling

- Do not mark task done on failing required checks.
- Document blockers and propose next action.
