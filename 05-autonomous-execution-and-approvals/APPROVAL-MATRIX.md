# Approval Matrix

**Status:** 🔴 RED — draft matrix; project-specific authority and evidence still need validation.

## Purpose
Make approval requirements predictable and consistent across the full 18-section method.

| Action category | Default rule | Minimum pre-action evidence | Approval record / scope limits |
|---|---|---|
| Read-only inspection and reporting within scope | Proceed | Target and purpose are clear | Task/scope record |
| Reversible, in-scope file edits | Proceed if included in approved task | Planned files, diff/review, validation plan | Approved task ID and bounded paths |
| Scope, product direction, or architecture change | Explicit approval | Impact, alternatives, dependencies, rollback implications | Approval ID, decision owner, affected requirement IDs |
| Destructive deletion or irreversible change | Explicit approval | Exact target, consequences, backup/rollback status | Approval ID, target, recovery evidence, execution window |
| Cost, paid plan, purchase, or financial commitment | Explicit approval | Amount/range, billing terms, alternatives | Approval ID, spending limit, renewal/cancellation terms |
| External messages, invitations, publication, or commitments | Explicit approval | Recipient/audience, complete content, timing, identity used | Approval ID, final content/version, recipient list, send window |
| Secrets, sensitive data, or privacy exposure | Stop and obtain explicit direction; apply security policy | Data classification, destination, minimum necessary disclosure | Security/privacy approval where permitted; never overrides law/policy |
| Permission, account ownership, security control, or production activation change | Explicit approval | Before/after state, risk assessment, verification and rollback plan | Approval ID, target environment, rollback owner, expiry/conditions |
| Test or release that can affect real users or live data | Explicit approval unless separately authorized by a documented release mandate | Environment, blast radius, monitoring, rollback | Applicable release mandate/approval ID, deployment window, go/no-go record |
| Unclear intent, conflicting instructions, or uncertain consequences | Pause and clarify | Concise description of ambiguity and safe options | Record blocker and decision required |

## Approval record schema
- Approval ID and lifecycle: PROPOSED / APPROVED / REJECTED / REVOKED / EXPIRED.
- Approver identity and authority source; approval timestamp and time zone.
- Exact action, target, environment, bounded scope, and excluded actions.
- Risks, consequences, alternatives, cost/recipient limits, and preconditions.
- Expiry/review trigger, revocation path, execution evidence, and final outcome.

## Approval quality
Approval must identify the action or bounded action set, target, and material consequences. A vague “continue” does not authorize a newly discovered destructive, costly, external, security-sensitive, or out-of-scope action.

## Revocation and expiry
A user may withdraw approval before execution. Approval for one project, environment, recipient, or time window does not automatically transfer to another. If material facts change, re-confirm.

## Dependencies
Use Sections 01–02 for scope and risks, Section 03 for engineering/security standards, Section 11 for privacy and secrets, and Sections 12–13 for status and blockers.

## Acceptance evidence
Test scenarios cover every category above, including ambiguous approval, changed conditions, and withdrawn approval. Record actual results before marking this section GREEN.

## Next action
Review the matrix against the autonomy boundaries and escalation protocol; resolve overlaps before real-project validation.
