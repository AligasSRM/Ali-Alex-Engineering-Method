# Security Test Plan

**Status:** 🔴 RED — plan template drafted; threat-specific tests pending.

## Purpose
Translate the threat model and security requirements into verifiable tests.

## Plan fields
- Test ID / run ID / linked threat, control, asset, and requirement IDs:
- Asset/threat and abuse scenario, exact target, and authorized scope:
- Security requirement and expected safe behavior.
- Affected boundary, route, service, or data store.
- Test method, prerequisites, test identity/data, and environment.
- Expected allow/deny/error outcome.
- Evidence to retain, test commit/configuration, expected result, and sensitive data to redact.
- Severity if the test fails.
- Rollback/containment plan and approval required.
- Owner and remediation/retest status.

## Test case register
| Test ID | Threat/control ID | Preconditions / identity | Environment / scope authorization | Expected safe behavior | Evidence/result | Finding owner / retest state |
|---|---|---|---|---|---|---|
| SEC-001 | TBD | TBD | TBD | TBD | TBD | TBD |

## Coverage areas
Authentication, authorization, tenant isolation, secret redaction, input validation, dependency failure, replay/idempotency, rate limiting, audit trails, privacy controls, and fail-closed behavior as relevant to the project.

## Execution controls
Do not test systems without authorization. Production security tests require a narrowly scoped approved plan and safe controls. Avoid destructive payloads or real personal data unless necessary and specifically authorized.

## Dependencies
Sections 03, 05, 09–10, and this section's threat model and access controls.

## Acceptance evidence
Every material threat maps to a test or a documented reason it cannot currently be tested, with residual risk visible.

## Next action
Create the project-specific threat-to-test map and run non-production checks first.
