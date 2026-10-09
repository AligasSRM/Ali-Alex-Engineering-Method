# Section 05 — Autonomous Execution and Approvals

**Status:** 🔴 RED — structure only; substantive work pending.

## Purpose
Define which tasks may proceed within approved scope and which require explicit human approval.

## Planned documents
- AUTONOMY-BOUNDARIES.md — permitted independent actions.
- APPROVAL-MATRIX.md — decisions requiring approval.
- HIGH-IMPACT-ACTIONS.md — destructive, costly, external, security-sensitive, or irreversible actions.
- CHANGE-CONTROL.md — scope and architecture change procedure.
- ESCALATION-PROTOCOL.md — uncertainty, conflicts, and blockers.
- ACCEPTANCE-CRITERIA.md — evidence required to complete this section.
- STATUS.md — current state and next action.

## Dependencies
Uses project scope and risk context from Sections 01–02.
## Authority and audit model
An approval is valid only when it identifies the exact action or bounded action set, target/environment, material consequences, approver, time/conditions, and durable evidence. Record an approval ID and link it from the change/task record. Re-check authorization if scope, target, recipient, cost, environment, or risk materially changes. A job title, role assignment, prior approval, or technical capability is not itself authorization.

## Guardrail
Never infer consent for material scope changes, costs, external communications, secret exposure, or destructive actions. Mandatory law, security/privacy controls, and fail-closed gates take precedence over a general approval.
