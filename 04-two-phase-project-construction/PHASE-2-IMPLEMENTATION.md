# Phase 2 — Incremental Implementation

**Status:** 🔴 RED — implementation workflow template only; no implementation is claimed.

## Entry gate
Begin only after the relevant structural blueprint, requirements, dependencies, and acceptance criteria are reviewed and approved.

## Per-increment workflow
1. Select one bounded unit of work and state its intended outcome.
2. Verify current repository/runtime/configuration state and relevant locked areas.
3. Identify impact, dependencies, security/privacy concerns, and rollback path.
4. Implement the smallest coherent change that meets the requirement.
5. Run focused tests, build/type/lint checks as applicable, and relevant regression tests.
6. Inspect the diff and verify no unrelated files or secrets were introduced.
7. Record exact commands, outcomes, failures, and remaining risks.
8. Request explicit approval for high-impact decisions or external actions.
9. Mark the increment complete only when acceptance evidence is recorded.

## Increment register
| ID | Requirement | Change scope | Tests / evidence | Regression impact | Approval needed | Outcome |
|---|---|---|---|---|---|---|
| INC-001 | TBD | TBD | TBD | TBD | TBD | Not started |

## Stop conditions
Stop if the baseline is unknown, a critical dependency is blocked, an unexpected destructive/security-impacting change appears, or required approval is missing. Report evidence and options rather than guessing.

## Acceptance criteria
- [ ] Each increment maps to an approved requirement.
- [ ] Baseline and change scope are documented.
- [ ] Required tests and regression checks pass or failures are explicitly reported.
- [ ] Diff and side effects are reviewed.
- [ ] Completion evidence and next action are recorded.
