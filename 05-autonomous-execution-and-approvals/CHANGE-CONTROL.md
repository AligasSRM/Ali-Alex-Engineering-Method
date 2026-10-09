# Change Control

**Status:** 🔴 RED — workflow drafted; decision records and cross-section traceability not yet tested.

## Purpose
Control changes to approved requirements, scope, architecture, dependencies, and section interfaces without losing continuity or breaking consistency across the 18-section method.

## Change workflow
1. **Describe:** record the requested or discovered change, reason, and source of evidence.
2. **Classify:** identify whether it is editorial, implementation-level and in-scope, or a material scope/architecture/security/cost/external-impact change.
3. **Trace:** list affected sections, files, requirements, dependencies, acceptance criteria, status gates, and downstream work.
4. **Assess:** compare current and proposed states, alternatives, risks, compatibility, migration/rollback, and test impact.
5. **Approve:** obtain explicit user approval for material changes before execution; record who approved what and any limits.
6. **Implement narrowly:** change only the approved scope and update linked documents where required.
7. **Verify:** run relevant checks and regression tests; review adjacent sections for consistency.
8. **Record and communicate:** update decision log, change summary, evidence, blockers, and next action.

## Change classes
- **Class A — editorial:** wording or formatting that does not alter meaning or obligations; preserve intent and review for consistency.
- **Class B — in-scope implementation:** a reversible change already authorized by accepted requirements; test and record it.
- **Class C — material:** changes scope, architecture, cost, external communications, security/privacy posture, production behavior, or irreversible state; pause for explicit approval.

## Rules
- Do not mark a section GREEN merely because its documents changed.
- Re-open a previously locked area only when evidence shows a defect, changed dependency, security risk, or regression that warrants it; record the reason.
- If a change affects a shared principle, update the authoritative source and trace dependent documents rather than making inconsistent local copies.

## Dependencies
Uses Sections 01–04 for identity, planning, standards, and phase gates; coordinate with Sections 12–15 for status, blockers, maintenance, and continuity.

## Acceptance evidence
A representative change is traced across all affected sections, approved at the correct level, tested, documented, and shown not to create unresolved contradictions.

## Next action
Validate the workflow with a non-destructive example, then align escalation and status reporting with the result.
