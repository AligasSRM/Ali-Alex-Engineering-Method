# Regression Plan

**Status:** 🔴 RED — plan drafted; project-specific coverage pending.

## Purpose
Choose repeatable checks that protect existing behavior after a change.

## Procedure
1. Identify the changed requirement, code/configuration, and affected interfaces.
2. Review dependencies and nearby workflows for indirect impact.
3. Select a targeted test that detects the original defect or requirement.
4. Select regression tests for adjacent high-risk behaviors.
5. Run static checks, unit/integration tests, contracts, E2E, security, and resilience checks as applicable.
6. Compare results with a known baseline where available.
7. Investigate failures and flaky results; do not suppress them to manufacture a pass.
8. Record tests omitted, why they were omitted, and residual risk.
9. Verify the final change set stays within approved scope.

## Change-to-regression matrix
| Change / commit ID | Requirement / defect / risk IDs | Affected paths / interfaces | Required test IDs | Baseline vs current result | Omitted tests and rationale | Residual risk / owner |
|---|---|---|---|---|---|---|
| CHG-001 | TBD | TBD | TBD | TBD | TBD | TBD |

## Risk priority
Prioritize authentication/access control, sensitive data, financial records, migrations, external integrations, and production-critical flows when affected.

## Dependencies
Sections 05–07, 09, and 11–17.

## Acceptance evidence
A change has a documented impact map, selected tests, actual results, and explicit coverage gaps.

## Next action
Use this plan during the cross-section patch review process.
