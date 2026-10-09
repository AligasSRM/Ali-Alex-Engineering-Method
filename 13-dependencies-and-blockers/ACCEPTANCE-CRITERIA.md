# Acceptance Criteria — Section 13

**Status:** 🔴 RED — criteria drafted; project-specific inventory pending.

- [ ] Internal and external dependencies have owners, versions/capabilities, and criticality.
- [ ] Dependency failure impacts and safe fallbacks are explicit.
- [ ] Active blockers have evidence, impact, owner, and next action.
- [ ] Escalation thresholds align with approvals and incident handling.
- [ ] Deferred work records residual risk, authority, and re-entry conditions.
- [ ] Cost, privacy, availability, and environment assumptions are verified or marked unknown.
- [ ] Secrets are referenced safely and never stored in dependency records.
- [ ] Registers are reconciled with project status and release readiness.

## GREEN gate
A real project has a reviewed dependency map and actionable blocker/deferral records with no hidden critical dependency.

## LOCKED gate
Lock only after GREEN, consistency review, and release-critical blockers are resolved or explicitly handled under authorized policy.

## Dependencies
Sections 02–03, 05–12, and 14–17.

## Next action
Populate and cross-check the registers against an actual project.
