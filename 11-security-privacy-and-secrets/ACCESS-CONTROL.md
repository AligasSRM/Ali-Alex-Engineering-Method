# Access Control

**Status:** 🔴 RED — policy drafted; system-specific authorization review pending.

## Purpose
Ensure identities can perform only the actions explicitly permitted for their role and context.

## Requirements
- Authenticate identities before protected operations.
- Enforce authorization server-side at every relevant boundary; do not rely on UI hiding alone.
- Apply least privilege and deny by default.
- Separate user, operator, administrator, service, and deployment identities where applicable.
- Validate tenant/resource ownership and prevent insecure direct object references.
- Protect privileged actions with appropriate re-authentication, approval, or audit.
- Revoke access promptly when no longer needed and periodically review privileges.
- Use secure session/token handling, expiry, and revocation appropriate to the system.
- Log security-relevant events without exposing credentials or sensitive payloads.

## Failure behavior
If required identity or authorization checks are unavailable or inconclusive, reject the protected operation safely. Do not silently grant access as a fallback.

## Dependencies
Sections 03, 05, 09–10, and 14–17.

## Acceptance evidence
Authorization tests cover allowed and denied cases, role boundaries, resource ownership, revocation, and failure behavior.

## Next action
Map roles and permissions to actual routes, APIs, resources, and privileged operations.
