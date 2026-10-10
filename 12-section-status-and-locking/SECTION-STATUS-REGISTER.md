# Section Status Register — Schema and Reconciliation Policy

**Status:** 🔴 RED — register specification; repository-wide reconciliation remains pending.

## Purpose
Define the fields and rules for a status register. This file is the **schema/policy template**, not the live 18-section status snapshot.

## Required columns
| Section | Status | Scope / commit SHA | Evidence IDs / links | Blocker / limitation | Owner / reviewer | Next action | Last reviewed (timestamp/time zone) |
|---|---|---|---|---|---|---|

## Source-of-truth model
The root snapshot is derived from the current section STATUS records and reviewed evidence; it must never be edited to imply a more optimistic state than the detailed record.
- The root `/SECTION-STATUS-REGISTER.md` is the current compact 18-section status snapshot.
- Each section's own `STATUS.md` records detailed section state, blockers, evidence, and next action.
- This Section 12 file defines the register's required fields and reconciliation rules; do not maintain a second competing live table here.
- If the root snapshot conflicts with a section record or supporting evidence, flag and resolve the discrepancy before reporting an overall status.
- Link each section to its `STATUS.md` and supporting evidence when the register format supports links.
- Never infer GREEN or LOCKED from file presence alone.
- Reconcile after status transitions and repository changes; record the tree/commit used for reconciliation and any mismatch found.

## Current baseline
The repository contains 18 section structures. Treat all as RED until substantive acceptance criteria are verified; confirm against live section records before relying on this baseline.

## Dependencies
All sections, especially Sections 09–10, 13, 15, and 17.

## Acceptance evidence
The root snapshot matches all 18 section records and links to current evidence.

## Next action
Complete the repository-wide reconciliation and record the result in `REPOSITORY-STRUCTURE-AUDIT.md`.
