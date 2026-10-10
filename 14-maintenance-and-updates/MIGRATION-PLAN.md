# Migration Plan

**Status:** RED — migration framework drafted; system-specific migration path pending.

## Migration identity and record
- Migration ID / linked requirement, dependency, and change IDs:
- Current and target commit/version/schema/configuration:
- Owner, reviewer, approver, and approved execution window/time zone:
- Expected duration/impact, affected consumers, and maintenance communication:
- Evidence/artifact location and final decision record:

## Required plan
- Objective, scope, owner, and approved change window.
- Current and target versions/configuration.
- Compatibility and data-format analysis.
- Affected dependencies and consumers.
- Backup or recoverable snapshot, where applicable.
- Preflight checks with expected outcomes, evidence links, and explicit GO / NO-GO criteria.
- Ordered migration steps and verification points.
- Rollback trigger, tested recovery procedure, and data reconciliation plan.
- Monitoring, communication, and post-migration validation.
- Evidence, approvals, and known limitations.

## Safety rules
A backup is considered recoverable only after a representative restore/recovery check or equivalent authoritative evidence. If rollback is impossible, the approver must explicitly accept that constraint before execution; define forward recovery and data reconciliation. Stop on any failed mandatory preflight check.

## Safety rules
Do not assume a backup is restorable without evidence. Do not run destructive migrations without authorization and a recovery plan. If rollback is impossible, state this before approval and plan forward recovery.

## Dependencies
Sections 05–07, 09–11, 13, and 17.

## Acceptance evidence
A migration plan is reviewed for compatibility, recoverability, verification, and failure handling.

## Next action
Draft a plan for one actual version or data change and test it safely.
