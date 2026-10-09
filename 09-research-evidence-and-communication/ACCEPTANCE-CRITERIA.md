# Acceptance Criteria — Section 09

**Status:** 🔴 RED — criteria drafted; practical review pending.

- [ ] Source hierarchy accounts for authority, freshness, relevance, and source limitations.
- [ ] Evidence log uses stable IDs, provenance, captured/checked timestamps and time zones, versions/commit/environment, scope, confidence, and both supporting and contradicting evidence.
- [ ] Claims are classified as facts, inferences, hypotheses, recommendations, decisions, plans, or unknowns.
- [ ] Status reports distinguish completed work from tested work, failures, blockers, and plans.
- [ ] Research stop rules record bounded scope, source/query coverage, stop reason, contradictions, and unresolved gaps without unsupported exhaustive claims.
- [ ] Section 06 troubleshooting rules and Section 05 approval gates are respected.
- [ ] No secrets or unnecessary personal data are included in evidence records.
- [ ] Time-sensitive claims have a review/expiry trigger and the date the source was last checked.\n- [ ] Status reports include repository/environment baseline and distinguish PASS, FAIL, BLOCKED, NOT CHECKED, and NOT APPLICABLE.\n- [ ] A real report can be audited from claim to source to conclusion.

## GREEN gate
Every applicable criterion has evidence; cross-section contradictions are resolved or tracked; a real report review passes.

## LOCKED gate
Lock only after GREEN, final review, and no known unresolved blocker or regression.

## Dependencies
Sections 03, 05–08, 10–13, and 17.

## Next action
Run an evidence-backed reporting walkthrough after the testing and release skeletons are available.
