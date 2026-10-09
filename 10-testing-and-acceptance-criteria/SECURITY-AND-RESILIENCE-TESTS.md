# Security and Resilience Tests

**Status:** 🔴 RED — test catalogue drafted; threat-specific coverage pending.

## Purpose
Verify safe behavior when permissions, dependencies, inputs, or infrastructure fail or are attacked.

## Test categories
- Authentication, authorization, least privilege, and tenant/data isolation.
- Input validation, injection resistance, and safe error responses.
- Secret handling and redaction in logs and artifacts.
- Rate limits, abuse controls, and resource exhaustion where relevant.
- Dependency timeouts, outages, partial failures, and malformed responses.
- Retry, idempotency, duplicate delivery, and recovery behavior.
- Backup/restore, rollback, and data integrity where applicable.
- Fail-closed behavior when a safety or authorization control is required but unavailable.
- Privacy-related access, retention, and deletion requirements.

## Security test record
- Test ID / linked threat, risk, and control IDs:
- Authorized scope, target, environment, and test window:
- Test account/data classification and blast radius:
- Expected safe/fail-closed behavior:
- Containment and rollback plan / responsible owner:
- Actual result, evidence, deviations, and residual risk:
- Approver/authorization evidence where required:

## Execution controls
Define scope, test accounts/data, environment, blast radius, and rollback before running intrusive tests. Security testing against live systems requires explicit authorization. Stop if a test risks real user data or unauthorized access.

## Dependencies
Sections 03, 05, 09, and 11–14.

## Acceptance evidence
A threat/risk-to-test map shows expected safe behavior and records results, limitations, and unresolved risks.

## Next action
Cross-check against Section 11 threat model and fail-closed rules.
