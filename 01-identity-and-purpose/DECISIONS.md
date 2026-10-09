# Decisions

**Status:** 🔴 RED — no substantive decisions approved yet.

Record each decision with:
- ID and date.
- Decision statement.
- Context and evidence.
- Options considered.
- Rationale and consequences.
- Approval status and approving party.
- Sections affected and review trigger.

## Decision log
No final product identity or scope decisions have been approved in this section yet.

### DEC-METHOD-001 — Account/registration documentation ownership
- **Date:** 2026-10-09
- **Decision:** Keep account/identity discovery in `01-identity-and-purpose/ACCOUNT-IDENTITY-AND-ACCESS-SCOPE.md`. Record each approved registration, sign-in, profile, recovery, session, and account-lifecycle requirement with a unique ID and verification method in Section 02's `REQUIREMENTS.md`. Keep security implementation controls in Section 11, acceptance tests in Section 10, approval gates in Section 05, and release evidence in Section 17.
- **Context/evidence:** The existing scope checklist already cross-links these sections; Section 02 already requires explicit account/identity dispositions and traceability. A separate numbered section would duplicate existing ownership.
- **Options considered:** Add Section 19; add a duplicate standalone registration checklist; use the existing scope and requirements files with explicit traceability.
- **Rationale:** The existing 18-section structure has clear owners for discovery, requirements, security, testing, approvals, and release. No distinct unowned responsibility has been demonstrated.
- **Consequences:** Do not add Section 19 for registration. Do not treat registration as approved for any specific product merely because the methodology documents it. Keep all affected sections RED until their own acceptance evidence passes.
- **Approval status:** Documentation placement decision recorded; product registration scope remains pending owner approval.
- **Affected sections:** 01, 02, 05, 10, 11, 12, 13, 17, 18.
- **Review trigger:** Revisit only if a real-project traceability review identifies a distinct responsibility that cannot be assigned to these existing sections.
