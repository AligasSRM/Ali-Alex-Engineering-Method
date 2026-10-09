# Delivery Plan

**Status:** 🔴 RED — planning template only; dates and sequencing are not approved.

## Phases and milestones
| Phase / increment ID | Outcome / requirement IDs | Prerequisites / blockers | Deliverables / affected paths | Verification gate / test IDs | Rollback / recovery | Owner | Target date | Status / evidence |
|---|---|---|---|---|---|---|---|
| Discovery and baseline | Approved understanding of current state | None | Discovery, audit, requirements draft | Owner review | TBD | TBD | Not started |
| Architecture and planning | Reviewed solution plan | Discovery and requirements | Architecture, dependencies, acceptance criteria | Planning review | TBD | TBD | Blocked pending discovery |
| Incremental implementation | Small, testable changes | Planning approval | Working increments | Tests and review per increment | TBD | TBD | Not started |
| Regression and release review | Evidence-backed release decision | Implemented scope | Test results, risk review, release notes | Release gate | TBD | TBD | Not started |

## Increment control and evidence
For each implementation increment, record the branch/PR or change reference, bounded file scope, approved requirement IDs, pre-change baseline, tests to run, rollback/recovery method, reviewer/approver where required, and evidence after execution. Do not label an increment complete based only on a commit existing.

## Risks and contingency
Record risk, likelihood, impact, trigger, mitigation, fallback, and owner. Dates must reflect actual constraints; do not invent commitments.

## Change management
Any scope, architecture, cost, security, or release-impacting change requires documented impact analysis and the required explicit approval.

## Acceptance criteria
- [ ] Sequencing reflects dependencies and verified constraints.
- [ ] Each phase has concrete deliverables and a verification gate.
- [ ] Risks, blockers, owners, and fallback actions are visible.
- [ ] Dates are confirmed rather than guessed.
- [ ] Project owner approves the plan before implementation begins.
- [ ] Each increment maps to approved requirements, dependencies, affected files, verification evidence, and a rollback/recovery approach.
- [ ] Blocked prerequisites are visible and cannot be bypassed by optimistic status labels.

## Next action
Complete after discovery, audit, requirements, and architecture are reviewed.
