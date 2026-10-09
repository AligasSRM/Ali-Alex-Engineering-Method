# Blocker Register

**Status:** 🔴 RED — template drafted; live blocker inventory pending.

## Required fields
- Stable blocker ID, lifecycle state (OPEN / INVESTIGATING / BLOCKED / RESOLVED / DEFERRED), and date/time/time zone created/updated.
- Blocker ID and concise description.
- Affected requirement, section, workflow, or release.
- Evidence IDs/links and date/time first observed; exact source/environment/commit where relevant.
- Severity, impact, and urgency.
- Accountable owner, decision/approval ID required, and escalation owner.
- Work blocked and safe work that may continue.
- Next diagnostic or resolution action.
- Target review date and escalation trigger.
- Resolution evidence and verification reviewer, or explicit authorized deferral ID with expiry/re-entry trigger.

## Rules
Link blockers to affected dependency/requirement/release IDs and record whether safe independent work can continue. Reassess severity when impact, scope, or evidence changes. A status change without new evidence does not close a blocker.

## Rules
A blocker remains open until resolution is verified or an authorized, risk-aware deferral is recorded. A lack of updates is not resolution. Escalate blockers that affect security, privacy, data integrity, external commitments, or release gates.

## Dependencies
Sections 05–06, 08–10, 12, and 17.

## Acceptance evidence
Every active blocker has evidence, impact, owner, next action, and a defined escalation path.

## Next action
Reconcile this register with status reports and release readiness.
