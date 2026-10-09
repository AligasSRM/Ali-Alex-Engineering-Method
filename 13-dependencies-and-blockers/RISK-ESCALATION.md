# Risk Escalation

**Status:** 🔴 RED — escalation rules drafted; thresholds need project review.

## Escalate promptly when
- A security/privacy boundary may be breached.
- Data integrity, recovery, or financial correctness is at risk.
- A production or external action may have irreversible consequences.
- A critical dependency fails without a safe fallback.
- A required approval is missing or the authorized scope is unclear.
- A release gate fails or evidence conflicts with the reported status.
- A blocker threatens a commitment or prevents a required safety check.

## Escalation record
- Risk/escalation ID, linked dependency/blocker/incident IDs, and timestamp/time zone:
Describe the evidence IDs, affected assets/users and environment, impact/likelihood/confidence, containment already taken, safe work that may continue, decision and approval IDs needed, accountable owner/approver, response expectation from the project's policy, and next review trigger. Redact secrets and unnecessary personal information.

## Response rules
Use the project's approved severity and response scheme; do not invent response-time promises. Record whether the risk blocks a specific activity/release and what evidence clears that block.

## Response rules
Contain immediate harm within existing authority; do not expand scope or take unapproved high-impact actions. Preserve evidence and follow the incident and approval procedures. Escalation does not itself authorize a risky change.

## Dependencies
Sections 05–06, 09–12, and 17.

## Acceptance evidence
Representative risk scenarios map to clear escalation thresholds, owners, and decisions.

## Next action
Review thresholds against the approval matrix and incident protocol.
