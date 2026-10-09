# Methodology Roadmap

**Status:** 🔴 RED — structure exists; cross-section audit and governance decisions remain open.

## Phase A — Structure
Create a consistent skeleton for all 18 sections, document responsibilities and dependencies, and define acceptance criteria without prematurely claiming completion.

## Phase A.1 — Cross-section compatibility gate
Before substantive implementation:
- Compare each section's purpose and declared dependencies with the other sections.
- Verify README file inventories against the live repository tree.
- Resolve dependency cycles and distinguish blocking prerequisites from coordination/reference links.
- Reconcile approval, security/privacy, testing, status/locking, documentation, and release gates.
- Confirm a single source-of-truth model for status and history records.
- Record findings, decisions, and evidence in `REPOSITORY-STRUCTURE-AUDIT.md`.
- Keep all sections RED until their applicable criteria are verified.

## Phase B — Substantive implementation
Only after the compatibility gate is resolved, return to Section 01 and complete it against its acceptance criteria. Verify evidence, mark GREEN only when all required criteria pass, then LOCK only under the agreed locking rules. Continue section by section.

## Governance
- Keep project-specific implementations separate from this methodology repository.
- Inspect existing state before edits.
- Record decisions, blockers, evidence, and next steps.
- Do not claim tests, integrations, or repository changes that have not been verified.
- Do not add secrets or confidential information to this public repository.
