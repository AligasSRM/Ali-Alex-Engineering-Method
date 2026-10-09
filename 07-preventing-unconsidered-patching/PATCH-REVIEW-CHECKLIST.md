# Patch Review Checklist

**Status:** 🔴 RED — checklist drafted; real change review pending.

Before approving or applying a patch, check:

- [ ] Does the change address an evidence-supported cause rather than only hiding a symptom?
- [ ] Is the scope minimal and within authorized requirements?
- [ ] Are affected files, services, interfaces, and downstream sections identified?
- [ ] Are security, privacy, performance, accessibility, and compatibility impacts considered?
- [ ] Are dependencies and runtime/version constraints understood?
- [ ] Is there a backup, rollback, or recovery strategy appropriate to the risk?
- [ ] Are new or changed tests specified?
- [ ] Are relevant existing tests and regression checks run?
- [ ] Are failures reported accurately, without masking or weakening tests to obtain a pass?
- [ ] Are required approvals recorded before high-impact action?
- [ ] Are documentation, decision records, and status registers updated?
- [ ] Is the final diff reviewed for unrelated changes and accidental secret exposure?

## Review outcome
Record **approve**, **revise**, or **reject**, with evidence and any conditions. A checklist alone does not prove a patch is safe.

## Dependencies
Sections 03, 05–06, 09–10, 11–14, and 17.

## Acceptance evidence
A real patch review has every applicable item checked with evidence and a recorded outcome.

## Next action
Cross-check with regression strategy and the design-repair options document.
