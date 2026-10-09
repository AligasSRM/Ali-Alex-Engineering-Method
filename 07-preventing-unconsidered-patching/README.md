# Section 07 — Preventing Unconsidered Patching

**Status:** 🔴 RED — structure only; substantive work pending.

## Purpose
Prevent symptom-only fixes and reduce regressions by requiring causal diagnosis and targeted verification.

## Planned documents
- ROOT-CAUSE-REQUIREMENT.md — evidence needed before a fix.
- PATCH-REVIEW-CHECKLIST.md — scope, rationale, side effects, and rollback.
- REGRESSION-STRATEGY.md — impacted tests and unaffected behavior.
- DESIGN-REPAIR-OPTIONS.md — when to fix architecture rather than patch symptoms.
- ACCEPTANCE-CRITERIA.md — evidence required to complete this section.
- STATUS.md — current state and next action.

## Dependencies
Works with Sections 06, 09, 10, and 14.
## Traceability and patch lifecycle
Link each proposed change to the Section 06 incident/diagnostic/root-cause record, Section 02 requirement IDs, Section 05 approval record where applicable, impacted paths/interfaces, Section 10 test evidence, and the resulting commit. Classify the change as **permanent fix**, **temporary mitigation**, **refactor**, or **architecture change**; record owner, reviewer, rollback/recovery, and revisit trigger.

## Guardrail
Disappearance of an error message alone does not prove the issue is fixed. A temporary mitigation is not a permanent resolution and must have explicit monitoring and expiry/review criteria.
