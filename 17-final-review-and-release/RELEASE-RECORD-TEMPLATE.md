# Release Record Template

**Status:** RED — template drafted; no release record completed.

## Record
- **Release record ID / release ID / status:**
- **Source repository / branch / exact commit SHA:**
- **Artifact digest/checksum or immutable build reference:**
- **Readiness evidence timestamp and reviewer:**
- **Release ID/name:**
- **Approved scope and version/commit:**
- **Artifact/build identifier:**
- **Target environment and deployment time:**
- **Release owner and approver:**
- **Readiness checklist/review evidence:**
- **Test and regression results:**
- **Open blockers and accepted residual risks:**
- **Deployment/migration steps and results:**
- **Post-release verification and observation window:**
- **Rollback/recovery status:**
- **User/operator communication:**
- **Decision:** GO / NO-GO / CONDITIONAL GO, with authority and scope
- **Conditions, owners, expiry/review timestamp, and failure/rollback trigger:**
- **Final outcome and follow-up actions:**

## Rules
A release record must not merge planned and observed facts. If deployment succeeds but post-release checks fail or are unavailable, record the deployment event and the separate verification failure/gap. Keep prior records and corrections auditable.

## Rules
Do not include secret values or unnecessary personal data. Distinguish approval, deployment, and successful post-release verification as separate events.

## Dependencies
Sections 05, 09–16, and 18.

## Acceptance evidence
The record provides a traceable account of what was approved, what was deployed, and what was verified.

## Next action
Use the template for a controlled non-production release exercise.
