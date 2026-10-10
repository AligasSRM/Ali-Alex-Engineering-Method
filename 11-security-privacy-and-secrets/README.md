# Section 11 — Security, Privacy, and Secrets

**Status:** 🔴 RED — structure only; substantive work pending.

## Purpose
Protect systems and data through risk-based controls, least privilege, secret handling, and explicit failure behavior.

## Planned documents
- THREAT-MODEL.md — assets, actors, trust boundaries, and threats.
- DATA-CLASSIFICATION.md — data categories and handling rules.
- SECRET-MANAGEMENT.md — storage, access, rotation, and exposure response.
- ACCESS-CONTROL.md — authentication, authorization, and least privilege.
- PRIVACY-CONTROLS.md — collection, retention, access, and deletion.
- FAIL-CLOSED-RULES.md — required behavior when safety or authorization checks fail.
- SECURITY-TEST-PLAN.md — verification approach.
- ACCEPTANCE-CRITERIA.md — evidence required to complete this section.
- STATUS.md — current state and next action.

## Dependencies
Applies across all project sections and deployments.
## Traceability and security decision model
Assign stable asset, data-flow, threat, control, exception, and test IDs. Link threats to controls, owners, verification evidence, residual risk, and release disposition. Record scope, environment, version, reviewer, and checked date for material security decisions. Separate implemented controls from planned controls and accepted residual risks.

## Cross-section precedence
Mandatory security/privacy and fail-closed controls cannot be overridden by general user approval, role assignment, GREEN/LOCKED status, or a release checklist. Validate the integrated scenarios in `13-dependencies-and-blockers/GOVERNANCE-PRECEDENCE-AND-SCENARIOS.md` before claiming the precedence model is verified.

## Guardrail
Never place credentials, private user data, or secrets in repository files or public logs. An exception cannot silently disable a mandatory control or override applicable law.
