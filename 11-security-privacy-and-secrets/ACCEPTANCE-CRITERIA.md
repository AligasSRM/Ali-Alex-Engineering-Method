# Acceptance Criteria — Section 11

**Status:** 🔴 RED — criteria drafted; project-specific security review pending.

- [ ] Threat model uses stable asset/flow/threat/control IDs, identifies actors and trust boundaries, and records likelihood, impact, owner, and residual risk.
- [ ] Data classification maps actual data categories to purpose, stores/processors, access, retention/deletion, backup/logging, and owners.
- [ ] Secret lifecycle covers storage, least privilege, redaction, rotation, revocation, and exposure response.
- [ ] Access control defines server-side authorization, least privilege, revocation, and safe failure behavior.
- [ ] Privacy controls cover purpose, minimization, sharing, retention, deletion, and applicable jurisdictional review.
- [ ] Fail-closed rules map each mandatory control and failure mode to explicit deny/limit behavior, audit signal, recovery owner, re-entry condition, and test ID.
- [ ] Security test plan covers material threats and records evidence safely.
- [ ] Section 05 approval requirements are respected for access changes and sensitive disclosures.
- [ ] Secret inventory contains metadata only; rotation/revocation evidence contains no secret values.\n- [ ] Security tests identify stable test/run IDs, authorized target/environment, expected safe behavior, evidence, and remediation owner.\n- [ ] Privacy/legal uncertainties are assigned to a qualified reviewer and treated as blockers when material.\n- [ ] A real project security review records findings, owners, residual risks, and follow-up.
- [ ] No credentials or unnecessary personal data appear in repository documentation or public logs.

## GREEN gate
Applicable controls are implemented or clearly assigned, test evidence exists, residual risks are explicit, and required review is complete.

## LOCKED gate
Lock only after GREEN, final review, and no unresolved release-critical security blocker.

## Dependencies
Sections 03, 05, 09–10, and 12–17.

## Next action
Perform a project-specific threat review and validate high-priority controls in a safe environment.
