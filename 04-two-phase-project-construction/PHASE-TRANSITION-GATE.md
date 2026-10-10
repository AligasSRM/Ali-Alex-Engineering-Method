# Phase Transition Gate

**Status:** 🔴 RED — gate template only; no phase transition has been approved.

## Gate A — Structure to implementation
- [ ] Scope and exclusions are approved.
- [ ] Structure/module inventory is complete for the agreed scope.
- [ ] Interfaces, dependencies, and ownership are documented.
- [ ] Requirements and acceptance criteria are traceable.
- [ ] Material risks and unresolved decisions have owners.
- [ ] Security/privacy/accessibility/operational concerns are assessed as applicable.
- [ ] Baseline and rollback constraints are known.
- [ ] Project owner explicitly approves the transition.

**Gate A decision record**
- Decision: NOT REVIEWED (PASS / FAIL / BLOCKED / NOT APPLICABLE)
- Scope and baseline branch/SHA: TBD
- Reviewer / accountable approver: TBD
- Evidence links and failed/skipped checks: TBD
- Exceptions, risk owner, and expiry/review date: TBD
- Decision date / next review trigger: TBD

## Gate B — Implementation increment to acceptance
- [ ] Requirement and intended behavior are clear.
- [ ] Change scope and impact are reviewed.
- [ ] Relevant automated and manual tests are completed.
- [ ] Regression and compatibility impact are checked.
- [ ] No unresolved critical failure or unapproved high-impact change remains.
- [ ] Evidence, limitations, and rollback/mitigation are recorded.
- [ ] Required reviewer/owner approval is recorded.

**Gate B decision record**
- Decision: NOT REVIEWED (PASS / FAIL / BLOCKED / NOT APPLICABLE)
- Increment ID and requirement IDs: TBD
- Baseline and resulting commit SHA: TBD
- Environment / exact verification commands: TBD
- Reviewer / accountable approver: TBD
- Evidence links, failures, and skipped checks: TBD
- Rollback/recovery readiness and exceptions: TBD
- Decision date / next review trigger: TBD

## Rule
A gate cannot pass based on intention or a checklist alone. Every checked item requires supporting evidence. Missing or ambiguous evidence means BLOCKED, not PASS. NOT APPLICABLE requires an explicit rationale and authorized reviewer. A failed mandatory security/privacy or approval gate cannot be waived by a general phase approval. Failure keeps the relevant work blocked or RED.
