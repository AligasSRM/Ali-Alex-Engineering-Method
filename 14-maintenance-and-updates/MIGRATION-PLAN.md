# Migration Plan

**Status:** RED — migration framework drafted; system-specific migration path pending.

## Required plan
- Objective, scope, owner, and approved change window.
- Current and target versions/configuration.
- Compatibility and data-format analysis.
- Affected dependencies and consumers.
- Backup or recoverable snapshot, where applicable.
- Preflight checks and explicit go/no-go criteria.
- Ordered migration steps and verification points.
- Rollback trigger, tested recovery procedure, and data reconciliation plan.
- Monitoring, communication, and post-migration validation.
- Evidence, approvals, and known limitations.

## Safety rules
Do not assume a backup is restorable without evidence. Do not run destructive migrations without authorization and a recovery plan. If rollback is impossible, state this before approval and plan forward recovery.

## Dependencies
Sections 05–07, 09–11, 13, and 17.

## Acceptance evidence
A migration plan is reviewed for compatibility, recoverability, verification, and failure handling.

## Next action
Draft a plan for one actual version or data change and test it safely.
