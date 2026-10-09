# Acceptance Criteria — Section 17

**Status:** RED — criteria drafted; integrated release exercise pending.

- [ ] Readiness checklist covers scope, tests, dependencies, security/privacy, operations, recovery, and approvals.
- [ ] Final review records evidence, findings, dispositions, and authorized decision.
- [ ] GO/NO-GO/CONDITIONAL GO rules cannot bypass mandatory controls.
- [ ] Rollback or forward recovery is realistic and tested where feasible.
- [ ] Post-release verification is tied to the deployed artifact and observation window.
- [ ] Release record distinguishes approval, deployment, and verified outcome.
- [ ] Residual risks and deferred work are reconciled with Section 13.
- [ ] Locked sections and required approvals align with Sections 05 and 12.
- [ ] A representative release/recovery exercise is reviewed.

## GREEN gate
A complete release lifecycle is traceable from readiness through final review, deployment, and post-release verification.

## LOCKED gate
Lock only after GREEN and successful review of the applicable release and recovery evidence.

## Dependencies
Sections 05–16 and 18.

## Next action
Run a controlled release simulation after the repository-wide structure review.
