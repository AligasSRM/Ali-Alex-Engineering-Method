# Status Transition Rules

**Status:** 🔴 RED — transition policy drafted; workflow review pending.

## Permitted transitions
- **RED → YELLOW:** work begins with defined scope, owner, and next action.
- **YELLOW → ORANGE:** work becomes blocked or paused, with evidence and a resume condition.
- **ORANGE → YELLOW:** the blocker is cleared or an approved safe path is established.
- **YELLOW → GREEN:** applicable acceptance criteria are met and evidence is reviewed.
- **GREEN → LOCKED:** final review, scope check, and required regression checks pass.
- **GREEN → RED:** a verified defect, changed requirement, failed regression, or material new risk invalidates the prior acceptance evidence.
- **GREEN → YELLOW:** new authorized work is in scope and prior acceptance remains valid for the unchanged scope.
- **LOCKED → YELLOW:** authorized repair/change work begins after impact review and explicit reopening; use this when the prior accepted baseline remains valid outside the bounded reopened scope.
- **LOCKED → RED:** evidence shows the locked acceptance itself is invalid, such as a reproduced critical defect or invalidated mandatory control.
- **ORANGE → RED:** the blocker cannot be safely resolved within the approved scope or the prior evidence is invalidated.

## Controls
A status transition record must include a stable event ID, section/scope/version, prior/new status, reason and trigger, supporting/contradicting evidence, reviewer/approver, timestamp, blocker/limitation, affected downstream sections, and next action. The root register is a derived snapshot, not an independent authority.

## Controls
Record prior/new status, reason, evidence, approver where required, date, and remaining risks. Never skip a gate merely to meet a deadline. Deferral alone does not resolve a blocker.

## Dependencies
Sections 05–07, 09–10, 13, 15, and 17.

## Acceptance evidence
A sample status history shows valid transitions with traceable reasons and evidence.

## Next action
Cross-check transitions against approval and release gates.
