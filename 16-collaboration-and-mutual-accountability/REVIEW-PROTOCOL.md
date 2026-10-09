# Review Protocol

**Status:** RED — protocol drafted; real review workflow pending.

## Review record
- Review ID / change, requirement, and commit IDs:
- Scope, environment, acceptance criteria, and evidence set:
- Reviewer identity / authority / independence assessment:
- Findings: stable ID, severity, evidence, affected scope, owner, due/review date:
- Disposition: ACCEPTED / FIX REQUIRED / BLOCKED / WAIVED BY AUTHORIZED DECISION (where lawful):
- Final diff/commit, regression result, decision, date/time/time zone:

## Review procedure
1. Confirm scope, version/commit, acceptance criteria, and reviewer authority.
2. Inspect the change and supporting evidence independently.
3. Check correctness, security/privacy, compatibility, maintainability, and downstream impact as relevant.
4. Verify tests and distinguish executed results from claims.
5. Record findings with severity, evidence, and actionable remediation.
6. Resolve or explicitly disposition findings under the approval policy.
7. Recheck the final diff and required regression after changes.
8. Record the decision, reviewer, date, and remaining risks.

## Independence
Document any relationship or prior involvement that could impair independence. Do not mark a finding waived solely because it is inconvenient; record the authorized risk owner, rationale, compensating controls, and expiry/review trigger.
High-impact security, privacy, financial, or release decisions require the reviewer independence specified by project policy. If independence is unavailable, record the limitation and obtain the required alternate approval; do not imply independent review occurred.

## Dependencies
Sections 05–07, 09–13, and 17.

## Acceptance evidence
A real change has a review record, traceable findings, and verified disposition.

## Next action
Apply the protocol to one representative change.
