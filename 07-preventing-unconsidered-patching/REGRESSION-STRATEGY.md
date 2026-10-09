# Regression Strategy

**Status:** 🔴 RED — strategy drafted; project-specific test mapping pending.

## Purpose
Verify that a change fixes the target issue without breaking related or previously working behavior.

## Procedure
1. Identify the defect and the expected corrected behavior.
2. Map the change to directly affected components, interfaces, data, and user flows.
3. Select a focused test that would fail before the fix and pass after it.
4. Select adjacent-behavior tests based on shared code, dependencies, and risk.
5. Run existing regression suites and relevant build, type, lint, security, and accessibility checks where applicable.
6. Record exact commands, environment, results, and failures.
7. Investigate failures rather than deleting, skipping, or weakening tests without justified review.
8. Compare final diff with approved scope and check rollback readiness.
9. If the test environment is incomplete, state the limitation; do not call the result fully verified.

## Impact-to-test matrix
| Change / requirement ID | Affected component / interface / data | Risk / failure mode | Test ID and type | Baseline expectation | Result / evidence link | Status / owner |
|---|---|---|---|---|---|---|
| CHG-001 | TBD | TBD | TBD | TBD | TBD | TBD |

Distinguish tests that failed before the fix, tests run after the fix, tests not run, and tests that were skipped with approved rationale. Record exact commands, tool versions, environment, exit status, and artifacts. A green aggregate suite does not excuse an unexplained failure in a critical targeted test.

## Risk-based coverage
Prioritize authentication/authorization, payments and financial records, data migrations, public APIs, security boundaries, and production-critical paths when affected.

## Dependencies
Sections 03, 05–06, 09–10, and 17.

## Acceptance evidence
A real change has a traceable impact-to-test map and documented results for all applicable checks.

## Next action
Use this strategy to review a representative patch after the remaining section structures are available.
