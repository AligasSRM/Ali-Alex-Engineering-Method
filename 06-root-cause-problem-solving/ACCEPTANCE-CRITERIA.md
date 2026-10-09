# Acceptance Criteria — Section 06

**Status:** 🔴 RED — criteria drafted; scenario validation pending.

- [ ] Incident intake captures environment, reproduction, impact, baseline, and evidence without secrets.
- [ ] Diagnostic protocol records competing hypotheses and discriminating tests.
- [ ] Attempts are materially distinct and evidence-led.
- [ ] After two failed distinct attempts, broader research occurs before any third implementation attempt.
- [ ] A failed third attempt produces a stop report and safe options, not an unrecorded retry loop.
- [ ] Research sources are dated, relevant to the installed version, and ranked by reliability.
- [ ] Root-cause claims are proportional to evidence; uncertainty is explicit.
- [ ] Proposed fixes include rollback and targeted regression strategy.
- [ ] Escalation and approval controls from Section 05 are respected.
- [ ] A real incident walkthrough is documented and reviewed.

## GREEN gate
Every applicable item has recorded evidence, cross-section contradictions are resolved or tracked, and the workflow passes a real incident walkthrough.

## LOCKED gate
Lock only after GREEN, final review, and no known unresolved regression or blocker. Reopen only with a recorded reason.

## Dependencies
Sections 05, 07–10, and 12–15.

## Next action
Run scenario validation after the relevant section skeletons are available.
