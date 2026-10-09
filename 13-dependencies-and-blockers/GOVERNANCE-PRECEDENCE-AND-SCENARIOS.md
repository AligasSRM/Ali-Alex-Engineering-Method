# Governance Precedence and Cross-Section Scenarios

**Status:** 🔴 RED — precedence model drafted; owner review and scenario execution pending.

## Purpose

Define how approval, security/privacy, status, dependency, and release gates interact when more than one applies to the same action. This document proposes a shared test oracle; it does not grant authority or approve a real operation.

## Precedence rules

Apply all relevant controls cumulatively. A lower-level pass cannot waive a higher-level requirement.

1. **Law, platform policy, and mandatory security/privacy constraints:** prohibited actions remain prohibited. A user approval cannot authorize an unlawful or policy-disallowed action.
2. **Explicit user approval and scope (Section 05):** obtain approval for approval-gated actions before execution. Approval must cover the exact action, target, environment, scope, and material consequences.
3. **Applicable security/privacy controls (Section 11):** satisfy mandatory controls and fail-closed requirements before affected operations. Approval does not override a mandatory control.
4. **Dependency/blocker gate (Section 13):** resolve blockers whose documented impact applies to the action or release. Unrelated blockers do not automatically stop safe, independent work.
5. **Status and acceptance evidence (Sections 10 and 12):** a GREEN/LOCKED label is valid only within the accepted scope and evidence. Invalidated evidence reopens the affected scope under the transition rules.
6. **Release authorization (Section 17):** production/live-user release requires all applicable prior gates, an authorized GO decision, a defined recovery path, and post-release verification. A release checklist cannot override approval or security gates.
7. **Role and reviewer assignment (Section 16):** role ownership enables execution/review only within delegated authority; a role title alone is not approval.
8. **Durable records and effective agreement (Sections 15 and 18):** record the decision, evidence, authority, scope, timestamp, and outcome. Draft methodology proposals do not silently override the last approved baseline.

When controls conflict, **pause the affected action**, record the conflicting requirements and evidence, and obtain a decision from the authorized owner. Do not resolve a conflict by choosing the least restrictive control.

## Scenario test matrix

| Scenario ID | Given / trigger | Expected decision | Required evidence | State |
|---|---|---|---|---|
| GOV-001 | User approval exists, but a mandatory security/privacy control fails | DENY/BLOCK; approval does not override the control | Approval ID, control/test ID, fail-closed outcome, owner | Not run |
| GOV-002 | Security checks pass, but the action requires approval and no valid approval exists | BLOCK until explicit scoped approval is recorded | Action scope, risk/impact, approval record | Not run |
| GOV-003 | A section is GREEN/LOCKED, but a material change invalidates its acceptance evidence | Reopen affected scope under Section 12; do not rely on stale status | Change/defect ID, invalidated evidence, transition event | Not run |
| GOV-004 | A role owner asks to perform an action outside their approval authority | BLOCK and route to authorized approver | Role/authority source, action scope, decision record | Not run |
| GOV-005 | A release checklist is complete, but an applicable critical blocker remains open | NO-GO for affected release; unrelated safe work may continue | Blocker impact, release decision, clearing criteria | Not run |
| GOV-006 | Tests pass, but required release approval is absent | NO-GO; tests do not authorize deployment | Test run IDs and missing approval gate | Not run |
| GOV-007 | A mandatory test/evidence item is unavailable or not checked | BLOCK the acceptance/release decision that requires it; never infer PASS | Missing-evidence record, owner, next action | Not run |
| GOV-008 | A blocker belongs to an unrelated component and has no impact on the current bounded task | Continue only if independence and safety are documented | Dependency ID, impact assessment, bounded scope | Not run |
| GOV-009 | An external message/publication is prepared and tests pass, but recipient/content approval is absent | Do not send/publish | Final content hash/version, recipient/audience, approval ID | Not run |
| GOV-010 | A proposed Section 18 method change conflicts with the effective approved baseline | Keep the approved baseline; defer proposal until authorized review and validation | Proposal ID, conflict analysis, approval/effective version | Not run |
| GOV-011 | Post-release critical verification fails or cannot be observed | Do not claim successful verification; invoke the recorded containment/recovery decision | Deployed artifact, observation evidence, incident/recovery record | Not run |
| GOV-012 | The user withdraws approval before execution or material facts change | Stop and re-confirm; do not rely on stale approval | Revocation/change event, new scope, renewed approval if needed | Not run |

## Execution record template

- Run ID / scenario ID / date and time zone:
- Repository, branch, exact commit, environment:
- Preconditions and scoped test target:
- Expected outcome:
- Actual outcome and evidence IDs:
- PASS / FAIL / BLOCKED / NOT RUN:
- Defect/finding ID, owner, and remediation:
- Reviewer and decision authority:
- Retest evidence and closure date:

## Acceptance gate

This document remains RED until an authorized owner approves the precedence rules, each applicable scenario is executed in a safe representative environment, failures are remediated and retested, and the dependency map and relevant Section 05/11/12/16/17/18 documents are reconciled. A written scenario table alone is not execution evidence.
