# Status Transition Rules

**Status:** 🔴 RED — transition policy drafted; workflow review pending.

## Permitted transitions
- **RED → YELLOW:** work begins with defined scope, owner, and next action.
- **YELLOW → ORANGE:** work becomes blocked or paused, with evidence and a resume condition.
- **ORANGE → YELLOW:** the blocker is cleared or an approved safe path is established.
- **YELLOW → GREEN:** applicable acceptance criteria are met and evidence is reviewed.
- **GREEN → LOCKED:** final review, scope check, and required regression checks pass.
- **GREEN/LOCKED → RED or YELLOW:** a verified defect, changed requirement, failed regression, or material new risk invalidates prior evidence.
- **LOCKED → YELLOW:** authorized change work begins after impact review and explicit reopening.

## Controls
Record prior/new status, reason, evidence, approver where required, date, and remaining risks. Never skip a gate merely to meet a deadline. Deferral alone does not resolve a blocker.

## Dependencies
Sections 05–07, 09–10, 13, 15, and 17.

## Acceptance evidence
A sample status history shows valid transitions with traceable reasons and evidence.

## Next action
Cross-check transitions against approval and release gates.
