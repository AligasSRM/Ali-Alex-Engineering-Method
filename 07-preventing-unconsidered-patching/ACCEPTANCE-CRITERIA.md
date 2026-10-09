# Acceptance Criteria — Section 07

**Status:** 🔴 RED — criteria drafted; practical review pending.

- [ ] Each patch has a stable ID linked to incident/diagnostic records, requirement IDs, baseline/resulting commit, owner, reviewer, and evidence.\n- [ ] Root-cause evidence and confidence are recorded before a permanent fix.
- [ ] Patch review covers scope, rationale, side effects, security/privacy, dependencies, rollback, tests, and approvals.
- [ ] Regression strategy maps each affected component/interface/data path to targeted and adjacent test IDs, environment, exact commands, results, and evidence.
- [ ] Test failures cannot be hidden by weakening or deleting checks without documented justification.
- [ ] Design repair options distinguish local correction, refactor, and architecture change.
- [ ] Material architecture/scope changes pause for explicit approval under Section 05.
- [ ] Cross-links to Sections 03, 05–06, 09–11, 13–14, and 17 are consistent.
- [ ] Temporary mitigations have monitoring, accountable owner, approval where required, expiry/review date, rollback, and permanent-fix trigger.\n- [ ] Patch review outcome is APPROVE / REVISE / REJECT / BLOCKED with conditions and residual risk.\n- [ ] A real change review includes evidence and a recorded outcome.

## GREEN gate
Every applicable criterion has evidence; a real patch walkthrough passes; contradictions are resolved or explicitly tracked.

## LOCKED gate
Lock only after GREEN, final diff review, and no known blocker/regression. Reopen only with documented cause.

## Next action
Validate on a real change after the full structure review.
