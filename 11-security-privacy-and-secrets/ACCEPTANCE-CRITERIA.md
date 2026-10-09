# Acceptance Criteria — Section 11

**Status:** 🔴 RED — criteria drafted; project-specific security review pending.

- [ ] Threat model identifies assets, actors, trust boundaries, entry points, and residual risk.
- [ ] Data classification defines handling rules for public, internal, confidential, and restricted information.
- [ ] Secret lifecycle covers storage, least privilege, redaction, rotation, revocation, and exposure response.
- [ ] Access control defines server-side authorization, least privilege, revocation, and safe failure behavior.
- [ ] Privacy controls cover purpose, minimization, sharing, retention, deletion, and applicable jurisdictional review.
- [ ] Fail-closed rules map mandatory controls to explicit behavior when checks fail or are unavailable.
- [ ] Security test plan covers material threats and records evidence safely.
- [ ] Section 05 approval requirements are respected for access changes and sensitive disclosures.
- [ ] A real project security review records findings, owners, residual risks, and follow-up.
- [ ] No credentials or unnecessary personal data appear in repository documentation or public logs.

## GREEN gate
Applicable controls are implemented or clearly assigned, test evidence exists, residual risks are explicit, and required review is complete.

## LOCKED gate
Lock only after GREEN, final review, and no unresolved release-critical security blocker.

## Dependencies
Sections 03, 05, 09–10, and 12–17.

## Next action
Perform a project-specific threat review and validate high-priority controls in a safe environment.
