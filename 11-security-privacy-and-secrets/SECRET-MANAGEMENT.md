# Secret Management

**Status:** 🔴 RED — control framework drafted; implementation and rotation paths unverified.

## Purpose
Prevent secret exposure and manage credentials throughout their lifecycle.

## Requirements
- Store secrets only in approved secret managers or protected environment configuration.
- Never hardcode secrets in repositories, examples, logs, issue reports, screenshots, or client-side bundles.
- Apply least privilege, narrow scope, and separate credentials by environment.
- Restrict read access; avoid unnecessary copying and display.
- Rotate credentials according to risk, provider requirements, and incident triggers.
- Revoke exposed or unused credentials promptly; investigate the exposure path.
- Keep placeholders clearly nonfunctional and never confuse them with real credentials.
- Validate secret presence and required permissions without printing secret values.
- Document owners, renewal expectations, recovery, and revocation paths without recording the secret itself.

## Secret inventory metadata (never the secret value)
Record secret/reference ID, purpose, owner, provider/store location, environment and scope, permission boundary, creation/last-rotation/next-review dates, expiry where applicable, renewal/revocation procedure, and dependency references. Never copy the secret value into this register.

## Exposure response
Stop further disclosure, preserve relevant evidence safely, revoke or rotate affected credentials, inspect access/audit records, assess impact, notify the appropriate owner, and verify the replacement works. Follow Section 05 for approvals where required, without delaying a clearly authorized containment action.

## Dependencies
Sections 03, 05, 09–10, and the access/privacy controls in this section.

## Rotation evidence
A rotation record identifies the credential/reference, triggering reason, authorized operator, timestamp, revocation/rotation steps, dependent services updated, post-rotation verification, and any failed consumer or residual exposure. Redact all secret material.

## Acceptance evidence
A real deployment demonstrates secure configuration, least-privilege access, redaction, and a tested rotation/revocation procedure.

## Next action
Audit the chosen secret store and test rotation in a non-production environment.
