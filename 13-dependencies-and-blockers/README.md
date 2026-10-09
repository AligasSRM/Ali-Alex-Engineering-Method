# Section 13 — Dependencies and Blockers

**Status:** 🔴 RED — structure only; substantive work pending.

## Purpose
Track dependencies and impediments without hiding unresolved risks or confusing deferral with resolution.

## Planned documents
- DEPENDENCY-REGISTER.md — dependency, owner, version, and criticality.
- DEPENDENCY-MAP.md — typed cross-section edges, sequencing rules, and unresolved cycle decisions.
- BLOCKER-REGISTER.md — impact, evidence, owner, and next action.
- EXTERNAL-SERVICE-DEPENDENCIES.md — vendors, APIs, and availability assumptions.
- RISK-ESCALATION.md — thresholds for escalation and approval.
- DEFERRED-WORK.md — accepted deferrals and re-entry conditions.
- ACCEPTANCE-CRITERIA.md — evidence required to complete this section.
- STATUS.md — current state and next action.

## Dependencies
Supports planning, architecture, integration, maintenance, and release.
## Single dependency/blocker model
Use stable dependency, edge, blocker, risk, external-service, and deferral IDs. The cross-section map owns typed section-to-section relationships; the dependency register owns project/runtime/provider dependencies; the blocker register owns unresolved impediments; the deferred-work log owns approved non-delivery decisions. Link records rather than maintaining duplicate status sources.

## Guardrail
A blocker may be deferred only when impact, authority, compensating controls, and re-entry conditions are documented and deferral is lawful and safe. Deferral does not clear a mandatory gate.
