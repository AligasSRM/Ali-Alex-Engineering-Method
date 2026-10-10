# Acceptance Criteria — Section 15

**Status:** RED — criteria drafted; continuity exercise pending.

- [ ] Documentation standards distinguish facts, assumptions, decisions, and unknowns.
- [ ] Material decisions have stable IDs, lifecycle state, rationale, authority/evidence, scope, affected requirement IDs, and revisit/expiry triggers.
- [ ] Handoff records include verified state, evidence, blockers, and a safe next action.
- [ ] Changelog/history uses stable change IDs and links requirement/decision, commit/PR, test evidence, and explicit saved/committed/tested/deployed/released state.
- [ ] Sensitive data and secrets are excluded or appropriately redacted.
- [ ] Canonical information has a clear source of truth, with project history in Section 15 and methodology versioning in Section 18.
- [ ] Documentation links and status claims match live repository evidence.
- [ ] Handoffs preserve exact repository/commit/worktree and current approval scope; a receiving operator verifies live state before action.\n- [ ] A pause/resume exercise succeeds without guessing or repeating completed work.

## GREEN gate
Documentation is accurate and traceable, and a real continuity exercise passes with evidence.

## LOCKED gate
Lock only after GREEN and final review of cross-section links and history.

## Dependencies
Sections 02, 05–14, 17, and 18.

## Next action
Run a practical handoff exercise after the full structure is available.
