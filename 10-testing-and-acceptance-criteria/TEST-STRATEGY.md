# Test Strategy

**Status:** 🔴 RED — draft strategy; project-specific validation pending.

## Purpose
Define a layered, risk-based approach to testing and objective completion evidence.

## Test layers
- **Static checks:** formatting, linting, type checking, dependency/policy checks where applicable.
- **Unit:** isolated logic and edge cases.
- **Integration:** interaction between components, storage, services, and boundaries.
- **Contract/API:** schemas, compatibility, authorization, error handling, and version assumptions.
- **End-to-end:** representative user or operator workflows.
- **Security/resilience:** access control, failure behavior, recovery, abuse cases, and safe defaults.
- **Regression:** previously working behavior likely to be affected.
- **Live verification:** only when explicitly authorized and safe; distinguish from mocks, local tests, and staging.

## Test plan record
| Requirement / risk ID | Test case ID / layer | Expected behavior / failure mode | Environment / data class | Owner / tool | Pass-fail oracle | Evidence/run ID | Coverage gap / disposition |
|---|---|---|---|---|---|---|---|
| REQ-001 / RISK-001 | TEST-001 / TBD | TBD | TBD | TBD | TBD | TBD | TBD |

## Planning
Map each requirement and risk to a test, expected result, environment, owner/tool, and retained evidence. Prioritize tests by impact and likelihood. Define stop conditions and data/production safety boundaries before execution.

## Rules
- Define pass/fail oracles before running the test; avoid changing expected results after observing the outcome without an approved requirement change.
- Record flaky tests, retries, quarantines, and skipped tests separately; none count as a clean pass without an approved, time-bounded disposition.
- Keep test data isolated and classify external side effects before running.

## Rules
A test proves only the behavior and environment it actually exercised. A passing build is not proof of functional correctness; a mock is not proof of live integration. Never weaken acceptance criteria merely to obtain a pass.

## Dependencies
Sections 01–03, 05–09, 11, and 17.

## Acceptance evidence
A real project has a traceable requirement/risk-to-test map and justified test coverage.

## Next action
Apply the strategy to a representative requirement and identify missing test layers.
