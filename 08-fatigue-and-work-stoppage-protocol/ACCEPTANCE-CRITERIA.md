# Acceptance Criteria — Section 08

**Status:** 🔴 RED — criteria drafted; pause/resume testing pending.

- [ ] Stop-work triggers cover repeated failures, unsafe uncertainty, fatigue, missing approval, and unreliable evidence.
- [ ] Checkpoint captures verified state, last known-good point, tests actually run, blockers, and next safe action.
- [ ] Resume procedure requires live-state inspection and comparison with checkpoint.
- [ ] Handoff notes distinguish completed work from plans, assumptions, and unverified claims.
- [ ] No stop/resume path bypasses Section 05 approval gates or Section 06 diagnostic limits.
- [ ] Relevant dependencies and status are updated at pause and resume.
- [ ] A real pause/resume or handoff walkthrough succeeds without guessing.
- [ ] Sensitive information is not copied into checkpoints unnecessarily.

## GREEN gate
Every applicable criterion has evidence and the real walkthrough succeeds. Document existence alone is insufficient.

## LOCKED gate
Lock only after GREEN, final consistency review, and no known unresolved blocker. Reopen with a documented reason.

## Dependencies
Sections 05–07 and 09–15.

## Next action
Run a pause/resume walkthrough after the remaining section skeletons are available.
