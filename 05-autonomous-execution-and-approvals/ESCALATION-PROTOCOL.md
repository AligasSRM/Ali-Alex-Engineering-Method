# Escalation Protocol

**Status:** 🔴 RED — draft protocol; response paths and timing need validation on real work.

## Purpose
Provide a predictable response when evidence is incomplete, requirements conflict, risks exceed approved boundaries, or execution is blocked.

## Trigger conditions
Escalate when:
- user intent or acceptance criteria are materially ambiguous;
- documents or instructions conflict;
- a dependency is missing, unavailable, or changed;
- an action may exceed approved scope or create cost, external impact, destructive effects, security/privacy exposure, or production risk;
- a test fails, regression appears, or evidence contradicts a claimed status;
- two materially different diagnostic attempts fail and the next attempt requires a broader strategy;
- the same issue begins repeating without new evidence.

## Escalation record
- Escalation ID and severity/urgency: TBD using the project's approved severity scheme.
- Trigger, affected action/system, environment, and accountable owner: TBD.
- Facts/evidence, hypotheses, unknowns, and last known-good state: TBD.
- Immediate containment/stop decision and risk of inaction: TBD.
- Decision required, approver, response expectation, and next review trigger: TBD.
- Resolution, verification evidence, and linked blocker/incident/change IDs: TBD.

Do not invent response-time promises. Set severity definitions and response expectations for the real project, including an owner and an escalation route if the expected response window is missed.

## Procedure
1. Stop only the affected unsafe or uncertain action; preserve unrelated safe progress.
2. Capture observable evidence, exact failure, affected component, and last known-good state.
3. Separate facts, hypotheses, unknowns, and assumptions.
4. State the impact of continuing, stopping, or reverting.
5. Offer the smallest set of safe options and identify any decision that requires explicit approval.
6. Resume only after the blocker is resolved or the user has selected an authorized path.
7. Record the outcome and update dependencies, status, and continuity notes.

## Diagnostic discipline
Do not repeat the same failed approach without a changed hypothesis or new evidence. After two materially different failed attempts, broaden research and reassess assumptions; any third attempt must be based on that new evidence. If it fails, stop the loop and report findings, remaining uncertainty, and alternatives.

## Communication standard
Escalations should be concise and actionable: what failed, evidence, impact, what was tried, what must be decided, and the recommended next step. Never claim a fix, test, or external action succeeded without confirmation.

## Dependencies
Works with Section 06 root-cause problem solving, Section 07 patch discipline, Section 08 fatigue/stoppage, Section 09 evidence/communication, and Sections 12–13 status/blocker handling.

## Acceptance evidence
Run scenarios for ambiguity, conflict, missing dependency, failed diagnostics, and a high-impact action. Verify the affected action pauses and the report distinguishes evidence from hypotheses.

## Next action
Cross-check this protocol against Sections 06–09 and confirm that each escalation trigger has a clear owner and outcome.
