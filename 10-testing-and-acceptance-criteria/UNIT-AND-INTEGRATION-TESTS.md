# Unit and Integration Tests

**Status:** 🔴 RED — test guidance drafted; implementation-specific test plan pending.

## Unit tests
Cover core rules, normal cases, boundary values, invalid inputs, error paths, and deterministic behavior. Keep tests focused and independent. Assert meaningful outcomes rather than implementation details that make safe refactoring difficult.

## Integration tests
Verify real component boundaries: persistence, configuration, service adapters, queues, authentication/authorization, and error propagation as applicable. Use isolated test resources and known fixtures. Confirm cleanup and prevent test data from reaching production.

## Test case record
For material tests, record stable test ID, linked requirement/risk/defect ID, fixture/data class, preconditions, expected result, actual result, dependency mock/stub versus real boundary, environment/tool version, and evidence. Include negative authorization and error-propagation cases wherever applicable.

## Quality requirements
- Include regression tests for fixed defects where practical.
- Verify both successful and rejected/failed operations.
- Avoid shared mutable state and order-dependent tests.
- Keep secrets out of fixtures and logs.
- State when a dependency is mocked or replaced.
- Record flaky tests and investigate rather than silently ignoring them.

## Dependencies
Sections 03, 06–07, 09, and 11.

## Acceptance evidence
A project-specific test set demonstrates expected behavior and important boundaries with reproducible results.

## Next action
Map unit and integration coverage to the requirements and failure modes.
