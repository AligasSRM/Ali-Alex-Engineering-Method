# Governance Scenario Test Results — Provisional Tabletop Pass

**Status:** 🟡 Provisional model check passed; owner approval and real-workflow validation remain pending.

## Test boundary

- **Run type:** deterministic, table-driven decision-model simulation in an isolated execution environment.
- **Purpose:** check that the proposed precedence rules produce the documented expected decision for representative inputs.
- **Not tested:** GitHub permissions, deployment systems, real approval capture, production security controls, external publication, live incident response, or actual release tooling.
- **Authority:** the proposed oracle is not owner-approved. These results do not authorize actions and do not make Section 13 GREEN.

## Results

| Run ID | Scenario | Input summary | Expected | Actual | Result |
|---|---|---|---|---|---|
| TABLETOP-001 | GOV-001 | Approval exists; mandatory security control fails | DENY/BLOCK | DENY/BLOCK | PASS |
| TABLETOP-002 | GOV-002 | Approval required but absent; security passes | BLOCK | BLOCK | PASS |
| TABLETOP-003 | GOV-003 | LOCKED scope has invalidated evidence | REOPEN AFFECTED SCOPE | REOPEN AFFECTED SCOPE | PASS |
| TABLETOP-004 | GOV-004 | Actor lacks approval authority | BLOCK / ROUTE TO AUTHORIZED APPROVER | BLOCK / ROUTE TO AUTHORIZED APPROVER | PASS |
| TABLETOP-005 | GOV-005 | Release-ready checklist with applicable critical blocker | NO-GO FOR AFFECTED RELEASE | NO-GO FOR AFFECTED RELEASE | PASS |
| TABLETOP-006 | GOV-006 | Tests pass; release approval absent | NO-GO | NO-GO | PASS |
| TABLETOP-007 | GOV-007 | Mandatory acceptance evidence unavailable | BLOCK ACCEPTANCE/RELEASE DECISION | BLOCK ACCEPTANCE/RELEASE DECISION | PASS |
| TABLETOP-008 | GOV-008 | Unrelated blocker; independence and safety documented | CONTINUE ONLY IF INDEPENDENCE AND SAFETY DOCUMENTED | CONTINUE ONLY IF INDEPENDENCE AND SAFETY DOCUMENTED | PASS |
| TABLETOP-009 | GOV-009 | External publication; content/audience approval absent | DO NOT SEND/PUBLISH | DO NOT SEND/PUBLISH | PASS |
| TABLETOP-010 | GOV-010 | Proposed method change conflicts with approved baseline | KEEP APPROVED BASELINE; DEFER PROPOSAL | KEEP APPROVED BASELINE; DEFER PROPOSAL | PASS |
| TABLETOP-011 | GOV-011 | Post-release verification fails | NO SUCCESS CLAIM; CONTAIN/RECOVER | NO SUCCESS CLAIM; CONTAIN/RECOVER | PASS |
| TABLETOP-012 | GOV-012 | Approval revoked or no longer valid at execution | STOP AND RE-CONFIRM | STOP AND RE-CONFIRM | PASS |

## Outcome

- **12/12 provisional decision-model checks passed; 0 failed.**
- This confirms only the consistency of this small simulated decision model against its expected outcomes. It is not an independent validation of the governance policy because the model and expected outcomes were derived from the same draft.
- The 12 scenarios in `GOVERNANCE-PRECEDENCE-AND-SCENARIOS.md` remain **Not run** for owner-approved representative workflow execution until the owner approves the oracle and a real or faithful workflow test harness is available.
- Next: review the precedence rules and scenario coverage with the authorized owner, then execute/retest against the actual approval, status, security, and release workflows. Keep Section 13 RED meanwhile.
