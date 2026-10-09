# Final Review Protocol

**Status:** RED — protocol drafted; integrated review pending.

## Review sequence
1. Freeze the proposed scope and identify the exact commit/version.
2. Compare implementation against requirements and acceptance criteria.
3. Review architecture, interfaces, dependencies, data flows, and cross-section impacts.
4. Inspect security/privacy controls, permissions, secrets handling, and failure behavior.
5. Review test evidence, regression results, skipped checks, and known defects.
6. Confirm documentation, handoff, monitoring, recovery, and support readiness.
7. Reconcile blockers, deferred work, residual risks, and approvals.
8. Record findings and resolve or explicitly disposition each one.
9. Verify the final diff and repeat affected checks after changes.
10. Issue a traceable GO/NO-GO decision within the reviewer's authority.

## Independence and integrity
Do not self-certify a check as independently reviewed when it was not. Do not infer success from a green badge alone if the underlying scope or evidence is unclear. Unresolved release-critical findings result in NO-GO unless an explicitly authorized policy permits a safe alternative.

## Dependencies
Sections 05–07, 09–16, and 18.

## Acceptance evidence
A complete review record identifies scope, reviewer, evidence, findings, approvals, and decision.

## Next action
Run an integrated review exercise once the section structures are complete.
