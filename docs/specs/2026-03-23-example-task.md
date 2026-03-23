# Task Spec: add export validation guard

## Background

The export workflow currently lacks an explicit validation guard before execution.

## Objective

Add a narrow validation step so malformed export input is rejected before the export job starts.

## Scope

- add one validation guard in the export flow
- return a clear error for invalid export input
- document the validation path if needed

## Non-goals

- redesign the export architecture
- change unrelated export formatting
- add broad refactors

## Target files or areas

- src/export/*
- tests/export/*

## Constraints

- preserve current valid export behavior
- keep changes minimal
- validation must be explicit

## Implementation approach

Add the smallest coherent guard near the entry point of the export flow.

## Validation plan

### Black-box checks
- valid input still exports successfully
- invalid input is rejected with a clear error

### White-box checks
- add only if validation logic branches in a regression-sensitive way

## Completion criteria

- malformed input no longer proceeds into export execution
- current valid exports continue to work
- validation result is explicit and reviewable

## Write-back candidates

- reusable export validation rule if it is stable and worth reusing