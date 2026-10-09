# Decision Log

**Status:** RED — log format drafted; decisions need repository-wide reconciliation.

## Required fields
- Lifecycle: PROPOSED / APPROVED / REJECTED / DEFERRED / SUPERSEDED / REOPENED.
- Decision ID and concise title.
- Date/time/time zone, status, accountable decision-maker, and approver authority/evidence.
- Context and problem being resolved.
- Options considered and evaluation criteria.
- Decision and rationale.
- Consequences, trade-offs, and residual risks.
- Linked requirement/risk/dependency IDs, affected sections/files, baseline/resulting commit, and tests/evidence.
- Approval evidence where required.
- Revisit trigger and superseding decision, if any.

## Rules
Approval applies only to the recorded scope, target, environment, conditions, and time window. Record expiry/revisit triggers for time-sensitive decisions. Superseding a decision must link the replacement and preserve the original rationale and consequences.

## Rules
Record material decisions close to the time they are made. Preserve superseded decisions rather than rewriting history. Separate a proposal from an approved decision, and link evidence instead of copying sensitive data.

## Dependencies
Sections 02, 05–07, 09, 12–14, and 18.

## Acceptance evidence
Material decisions are traceable to their rationale, authority, and affected scope.

## Next action
Review existing decision records and normalize them without altering the substance of prior approvals.
