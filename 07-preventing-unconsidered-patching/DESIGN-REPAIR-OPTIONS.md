# Design Repair Options

**Status:** 🔴 RED — decision framework drafted; examples require review.

## Purpose
Help decide whether a defect needs a local fix, a broader refactor, or an architectural change.

## Decision levels
- **Local correction:** use when evidence identifies a narrow defect and the surrounding design remains sound.
- **Refactor:** consider when duplication, unclear boundaries, or coupling repeatedly causes similar defects and a bounded refactor reduces risk.
- **Architecture change:** consider when requirements cannot be met reliably within the current design or persistent systemic evidence justifies changing a major boundary.

## Decision record
- Decision ID / linked incident, patch, and requirement IDs:
- Current state and evidence supporting the proposed level:
- Alternatives considered and why rejected/deferred:
- Risk, cost, compatibility, migration, rollback, and verification impact:
- Decision state: PROPOSED / APPROVED / REJECTED / DEFERRED / SUPERSEDED:
- Owner / approver / date / revisit trigger:

## Evaluation criteria
Compare root-cause evidence, user impact, recurrence, complexity, security/privacy risk, compatibility, migration cost, reversibility, testability, schedule, and long-term maintenance. Record at least one viable alternative and why it was not selected.

## Approval gate
A major architecture or scope change requires explicit approval under Section 05 before implementation. Do not smuggle an architecture change into a “small patch.”

## Dependencies
Sections 01–05, 06, 09–10, and 14.

## Acceptance evidence
A real defect decision includes evidence, alternatives, trade-offs, approval where required, and a verification/rollback plan.

## Next action
Validate the decision framework against both a narrow defect and a recurring systemic defect.
