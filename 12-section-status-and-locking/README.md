# Section 12 — Section Status and Locking

**Status:** 🔴 RED — structure only; substantive work pending.

## Purpose
Standardize lifecycle labels and evidence required for status transitions.

## Planned documents
- STATUS-DEFINITIONS.md — RED, YELLOW, ORANGE, GREEN, LOCKED.
- TRANSITION-RULES.md — allowed status changes.
- GREEN-EVIDENCE-CHECKLIST.md — acceptance and verification evidence.
- LOCK-AND-REOPEN-PROTOCOL.md — lock criteria and justified reopening.
- SECTION-STATUS-REGISTER.md — central section tracker.
- ACCEPTANCE-CRITERIA.md — evidence required to complete this section.
- STATUS.md — current state and next action.

## Dependencies
Governance layer across the full methodology.
## Single status source and transition history
The root `SECTION-STATUS-REGISTER.md` is the compact cross-section snapshot; each section's `STATUS.md` is its detailed record; this directory defines policy and schema only. Every transition must record the scope/version, prior and new status, reason, evidence IDs/links, owner/reviewer/approver where required, timestamp, blockers, and next action. Reconcile the root snapshot to the detailed records after status-changing commits.

## Guardrail
Status colors communicate verified state; they do not substitute for evidence. Unknown or stale evidence cannot justify an optimistic status.
