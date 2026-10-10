# Requirement Traceability Matrix

**Status:** 🔴 RED — canonical matrix schema created; no project-specific requirements have been baselined or verified.

## Purpose and ownership

Section 02 owns the canonical link from an approved user/business need to its requirement, planned design/implementation increment, verification evidence, and release disposition. Other sections reference requirement IDs rather than maintaining competing copies of the requirement itself.

- Section 01 owns the problem, users, purpose, boundaries, and explicit account/identity scope decision.
- Section 02 owns requirement wording, priority, approval, and this traceability record.
- Section 03 owns technology/standard decisions made to satisfy requirements.
- Section 04 owns structure blueprints and bounded implementation increments.
- Section 05 owns approvals for gated decisions/actions.
- Section 10 owns test strategy, execution results, and test evidence.
- Section 11 owns security/privacy controls and sensitive-data handling.
- Section 12 owns status transition and GREEN/LOCKED evidence rules.
- Section 13 owns dependency/blocker records.
- Section 17 owns release readiness and go/no-go evidence.
- Section 15 owns durable decisions, handoffs, and history.

## Matrix schema

Create one row per requirement or explicitly grouped acceptance unit. Split requirements when one row would require materially different owners, priorities, or verification outcomes.

| Requirement ID | User need / source | Requirement and rationale | Priority | Owner / approver | Design / architecture reference | Implementation increment / files | Dependencies / risk | Verification method / test IDs | Evidence location / commit | Status | Release disposition / exception |
|---|---|---|---|---|---|---|---|---|---|---|---|
| REQ-001 | TBD | TBD — draft only; do not treat as approved | TBD | TBD | TBD | TBD | TBD | TBD | TBD | Draft | Not reviewed |

## Lifecycle and rules

1. Assign a stable unique ID before implementation; do not reuse retired IDs.
2. Record the source and intended user/business outcome. Mark the source as observed evidence, user request, contractual/policy requirement, or hypothesis.
3. Use explicit lifecycle states: **Draft → In Review → Approved → In Implementation → Verified → Accepted**. Use **Deferred**, **Rejected**, or **Superseded** with rationale when applicable.
4. Approval must identify the authorized owner and evidence. A drafted row is not an approved requirement.
5. Each approved requirement must have measurable or observable acceptance criteria and a verification method. Security, privacy, accessibility, reliability, support, and release concerns must be included where applicable.
6. Before changing scope or architecture, record impact on linked requirements, files, dependencies, tests, privacy/security, cost, schedule, and rollback; follow Section 05 change-control/approval rules.
7. Test evidence must identify the actual environment, command or procedure, result, date/commit, limitations, and artifact/reference. A planned test is not a passed test.
8. If a requirement is not applicable, record the rationale and authorized decision rather than leaving the row ambiguous.
9. Release disposition must be explicit: required before release, accepted exception with owner/expiry/mitigation, deferred to a named later milestone, or not applicable with rationale.
10. Never store secrets, private user data, or sensitive incident content in the matrix; link to an authorized evidence location.

## Change-impact review

For each material requirement change, record:
- Changed requirement ID and version/date.
- Before/after wording and reason.
- Affected design pages/modules/routes and repository paths.
- Dependency and blocker impact.
- Test additions/changes and regression coverage.
- Security/privacy/accessibility/operational impact.
- Approval evidence, commit/PR, and rollback or mitigation if applicable.

## Review checklist

- [ ] IDs are unique and stable.
- [ ] Every approved requirement has an accountable owner and approval evidence.
- [ ] Requirement wording is testable and its source/rationale is recorded.
- [ ] Design and implementation references point to real files/records or are explicitly pending.
- [ ] Dependencies and blockers are recorded in Section 13 rather than hidden in prose.
- [ ] Verification methods map to Section 10 test IDs and evidence.
- [ ] Security/privacy-sensitive requirements reference Section 11 controls and tests where applicable.
- [ ] Status and acceptance claims follow Section 12 and do not infer GREEN/LOCKED.
- [ ] Release-critical requirements map to Section 17 release evidence.
- [ ] Deferred/rejected/exception decisions include rationale, authority, owner, and revisit trigger where appropriate.

## Dependencies

Sections 01, 03–05, 09–13, 15, and 17. This matrix supports traceability; it does not replace their detailed source documents.

## Next action

Populate the matrix only after the project discovery and scope have been reviewed. Keep the example row marked Draft until the owner approves real requirement content and verification evidence.
