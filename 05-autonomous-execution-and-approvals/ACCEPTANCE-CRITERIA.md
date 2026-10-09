# Acceptance Criteria — Section 05

**Status:** 🔴 RED — criteria drafted; not yet exercised against a real project.

## Required checks
- [ ] Autonomy boundaries distinguish safe in-scope work from approval-required actions.
- [ ] Approval matrix covers scope/architecture changes, deletion, cost, external communication, security/access, privacy/secrets, production/live data, and ambiguous intent.
- [ ] High-impact catalogue includes pre-action impact, target, rollback, and approval checks.
- [ ] Change-control process traces downstream sections and files before material edits.
- [ ] Escalation protocol preserves evidence, separates facts from hypotheses, and prevents repeated blind attempts.
- [ ] Cross-links to Sections 01–04 and 06–17 are consistent with their stated responsibilities.
- [ ] No document implies that silence, technical capability, or a broad “continue” grants unlimited consent.
- [ ] A non-destructive walkthrough validates the process end-to-end.
- [ ] Any approval-gated scenario is paused before action unless a specific, applicable authorization is already recorded.
- [ ] Evidence, unresolved gaps, and next actions are documented.

## GREEN gate
Mark this section GREEN only after every applicable check has evidence, cross-section contradictions are resolved or explicitly tracked, and a real-project walkthrough passes. Document creation alone is not sufficient.

## LOCKED gate
LOCK only after GREEN, review of the final change set, and a recorded decision that no known blocker or regression remains. Reopen only with documented justification.

## Dependencies
Sections 01–04 define scope, planning, engineering standards, and phase gates. Sections 06–17 provide connected operating controls that must be cross-checked during the whole-structure review.

## Next action
Run the initial cross-section consistency review after the remaining section skeletons exist.
