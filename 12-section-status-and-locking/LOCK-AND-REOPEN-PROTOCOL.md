# Lock and Reopen Protocol

**Status:** 🔴 RED — protocol drafted; practical use pending.

## Lock requirements
A section may be LOCKED only after:
1. GREEN criteria are met with inspectable evidence.
2. Final review checks scope, dependencies, and unresolved risks.
3. Required regression checks pass for the locked change.
4. The exact reviewed version/commit and evidence are recorded.
5. Required approval is obtained.

## Reopen triggers
Reopen only for a documented reason: reproduced defect, failed regression, material security/privacy issue, changed requirement, invalidated dependency, or credible new evidence affecting acceptance.

## Reopen procedure
- Record the trigger and evidence.
- Identify affected scope, downstream sections, and release risk.
- Obtain approval when Section 05 requires it.
- Change LOCKED to YELLOW or RED as appropriate.
- Preserve prior decisions and test records.
- Implement the smallest safe correction and rerun affected regression checks.
- Re-lock only after the original gate is satisfied again.

## Dependencies
Sections 05–07, 09–10, 13, 15, and 17.

## Acceptance evidence
A sample reopen case explains the trigger, affected scope, and evidence required to re-lock.

## Next action
Review against real change-control and incident scenarios.
