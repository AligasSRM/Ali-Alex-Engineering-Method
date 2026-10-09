# Rollback and Recovery

**Status:** RED — recovery framework drafted; actual procedures untested.

## Recovery record
- Recovery/rollback ID and linked release/change/incident IDs:
- Trigger threshold and source of detection:
- Exact affected version/artifact/environment and data scope:
- Authorized decision-maker, recovery owner, and communications owner:
- Tested recovery evidence, prerequisites, and known limitations:
- Expected service/data integrity checks and pass/fail oracle:
- Actual outcome, timestamps, evidence links, and residual risk:

## Required plan
- Release/change identifier and affected components.
- Failure signals and explicit rollback/recovery trigger.
- Authorized decision-maker and on-call owner.
- Safe, ordered recovery steps and verification after each critical step.
- Data consistency and reconciliation plan.
- Backup/snapshot provenance and demonstrated restore evidence where relevant.
- External-provider, migration, and irreversible-action constraints.
- User/customer communication requirements.
- Monitoring after recovery and conditions to resume normal operations.
- Evidence capture and post-incident review.

## Rules
Distinguish a documented procedure from a successfully rehearsed recovery. Record whether rollback is technically possible for each stateful or external action; where not possible, define forward recovery and compensating action before release approval.

## Rules
- Prefer a tested recovery path over an assumed one.
- Do not promise rollback where schema, data, or external actions make it impossible.
- For irreversible changes, define forward recovery and compensating actions before approval.
- Preserve relevant evidence while protecting secrets and personal data.
- Reopening a locked section follows Section 12.

## Dependencies
Sections 05–08, 10–14, and 16.

## Acceptance evidence
A representative recovery exercise demonstrates that the plan is executable, authorized, and verifies data/service health.

## Next action
Exercise recovery in a non-production environment and record gaps.
