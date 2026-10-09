# Acceptance Criteria — Section 10

**Status:** 🔴 RED — criteria drafted; real test plan and run pending.

- [ ] Requirements and material risks map to appropriate test layers.
- [ ] Unit and integration coverage includes normal, boundary, and failure cases.
- [ ] Contract and E2E tests identify interfaces, workflows, and environment.
- [ ] Security/resilience tests align with Section 11 risks and fail-closed requirements.
- [ ] Regression plan covers direct and indirect impact.
- [ ] Evidence records exact commands, versions, results, failures, and limitations.
- [ ] Mocked, staging, and live verification are clearly distinguished.
- [ ] Approval and safety gates are respected for intrusive or production testing.
- [ ] No test is weakened or skipped without documented rationale and risk acceptance.
- [ ] A representative project test plan is reviewed and its results are traceable.

## GREEN gate
All applicable criteria have evidence, test gaps and limitations are explicit, and the project-specific review passes.

## LOCKED gate
Lock only after GREEN, final change-set review, and no unresolved release-critical blocker or regression.

## Dependencies
Sections 01–09, 11–13, and 17.

## Next action
Run a requirement-to-test traceability review after the security and release sections are structured.
