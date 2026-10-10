# Stop-Work Triggers

**Status:** 🔴 RED — draft; operational scenarios pending.

## Purpose
Define when to stop execution before repeated effort, fatigue, uncertainty, or risk degrades decision quality.

## Stop or pause when
- Two materially different diagnostic attempts fail and broader research is required by Section 06.
- A third evidence-based attempt fails; report and stop the loop.
- The same action is being repeated without new evidence or a changed hypothesis.
- Required authorization is missing or scope is unclear.
- Evidence conflicts with the claimed state, a regression appears, or data integrity is uncertain.
- A proposed step risks irreversible loss, cost, external communication, security/privacy exposure, or production impact without approval.
- Fatigue, rushed decision-making, or loss of context makes safe verification unreliable.
- The working environment or tools are too unstable to establish trustworthy results.

## Stop record
- Stop ID / related incident, attempt, approval, or blocker IDs:
- Trigger and affected action/component/environment:
- Timestamp/time zone and operator/owner:
- Last known-good state and exact evidence preserved:
- Work intentionally left incomplete / unsafe actions not performed:
- Required decision/approval and escalation owner:
- Next safe action, expected result, and re-entry condition:

## At the stop point
Preserve safe progress, capture exact evidence, record last known-good state, separate facts from assumptions, list blockers, and identify the smallest safe next action. Do not mark work GREEN or LOCKED while critical evidence is missing.

## Re-entry rule
Resume only after the triggering condition is resolved or explicitly contained, the live baseline is rechecked, required approval is current, and the next action is bounded. A checkpoint alone does not satisfy a blocked safety or authorization gate.

## Safety exception
Do not delay an already-authorized, proportionate containment action for an active incident; do not infer permission for unrelated high-impact remediation. Escalate when authority is unclear.

## Dependencies
Sections 05–07, 09–10, and 12–15.

## Acceptance evidence
Scenario walkthroughs show that unsafe loops stop, evidence is preserved, and the next action is clear.

## Next action
Use this trigger list to populate the checkpoint and resume templates.
