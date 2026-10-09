# Acceptance Criteria — Section 13

**Status:** 🔴 RED — criteria drafted; project-specific inventory pending.

- [ ] Internal and external dependencies have stable IDs, owners, versions/capabilities, criticality, source/check date, failure behavior, and recovery owner.
- [ ] The cross-section dependency map classifies each edge as blocking, coordination/reference, downstream consumer, or cross-cutting control.
- [ ] Every cross-section edge has a stable ID, typed relationship, exact output/gate, owner, validation evidence, and status; blocking edges have clearing evidence and no unresolved blocking cycle.
- [ ] Dependency failure impacts and safe fallbacks are explicit.
- [ ] Active blockers have lifecycle state, evidence IDs, impact, owner, next action, escalation route, and verification-based closure.
- [ ] Escalation thresholds align with approvals and incident handling.
- [ ] Deferred work records residual risk, authority/approval ID, expiry/review, and re-entry conditions; expiry does not auto-renew.
- [ ] Cost, privacy, availability, and environment assumptions are verified or marked unknown.
- [ ] Secrets are referenced safely and never stored in dependency records.
- [ ] Dependency, blocker, and deferral registers are reconciled with project status and release readiness; mandatory gates are never cleared by deferral.

## GREEN gate
A real project has a reviewed dependency map and actionable blocker/deferral records with no hidden critical dependency.

## LOCKED gate
Lock only after GREEN, consistency review, and release-critical blockers are resolved or explicitly handled under authorized policy.

## Dependencies
Sections 02–03, 05–12, and 14–17.

## Next action
Populate and cross-check the registers against an actual project.
