# Acceptance Criteria — Section 12

**Status:** 🔴 RED — criteria drafted; repository-wide transition audit pending.

- [ ] All five status labels have clear definitions.
- [ ] Status transitions and evidence/approval requirements are documented with a stable transition event record and current scope/commit.
- [ ] GREEN requires evidence for applicable acceptance criteria.
- [ ] LOCKED requires final review and relevant regression checks.
- [ ] Reopening requires a documented, evidence-backed trigger and a consistent destination state: YELLOW for bounded repair with unaffected acceptance intact, RED when prior acceptance is invalid, ORANGE when blocked.
- [ ] Status history preserves previous decisions and versions.
- [ ] Central register matches live section-level records at a recorded repository commit, with discrepancies resolved or explicitly blocked.\n- [ ] Evidence freshness is checked against the candidate commit/environment; stale evidence cannot support GREEN/LOCKED without revalidation.
- [ ] Status rules agree with approval, testing, and release sections.
- [ ] Sample transition and reopen flows pass review, including invalidated GREEN evidence and a bounded LOCKED reopen.

## GREEN gate
Definitions and transitions are consistent, tested against representative cases, and supported by evidence.

## LOCKED gate
Lock only after GREEN, register reconciliation, and final governance review.

## Dependencies
Sections 05–10, 13, 15, and 17.

## Next action
Audit transitions and the register after all section structures exist.
