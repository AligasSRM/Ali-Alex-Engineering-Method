# Method Evolution Policy

**Status:** RED — evolution policy drafted; feedback and outcome evidence pending.

## Purpose
Improve the method from real outcomes without turning every incident into an unreviewed rule change.

## Improvement inputs
- Verified incidents and root-cause reports.
- Failed or repeated acceptance checks.
- Review findings, escaped defects, and regression results.
- Handoff failures, unclear ownership, and repeated blockers.
- User feedback and documented usability friction.
- Changes in technology, security expectations, regulation, or delivery context.

## Proposal record
- Proposal ID / lifecycle: PROPOSED / UNDER REVIEW / APPROVED / REJECTED / DEFERRED / SUPERSEDED.
- Evidence/incident/lesson IDs and recurring-pattern assessment:
- Affected sections/files, dependency edges, and approval rules:
- Expected benefit, cost, risk, and compatibility/migration impact:
- Validation scenario, pass/fail criteria, and owner:
- Reviewer/approver, effective version/date, and revisit trigger:

## Improvement workflow
1. Record the observed problem and supporting evidence.
2. Distinguish a one-off event from a recurring or systemic pattern.
3. Identify root cause and affected method sections.
4. Propose a bounded change with expected benefit, cost, and risk.
5. Check conflicts, duplicate rules, and downstream dependencies.
6. Obtain approval where required.
7. Update versioned source documents and changelog.
8. Validate the change against a real or representative scenario.
9. Record outcome, unintended effects, and revisit triggers.

## Guardrails
Do not make a proposed rule effective merely because its document was edited or merged. Preserve the prior effective baseline until approval and required validation are recorded. Any conflict with mandatory legal, safety, security/privacy, or user-approval controls blocks adoption until resolved through an authorized path.
Do not claim a method improvement based only on intuition. Preserve prior versions and rationale. Do not weaken security, approval, evidence, or user-authority protections to improve speed.

## Dependencies
Sections 06–10, 12–17, and the working agreement.

## Acceptance evidence
A proposed change has traceable evidence, impact analysis, approval, validation, and a recorded outcome.

## Next action
Define a baseline and review cadence after the first real project has exercised the method.
