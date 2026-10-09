# Architecture Overview

**Status:** 🔴 RED — architecture template only; no architecture is approved.

## System context
- Product/system purpose: TBD from approved discovery.
- Users and external actors: TBD.
- System boundary: TBD.
- External integrations and trust boundaries: TBD.

## Component inventory
| Component / ID | Responsibility / linked requirement IDs | Inputs / outputs / data classification | Dependencies / trust boundary | Failure behavior / recovery |
|---|---|---|---|---|
| TBD | TBD | TBD | TBD | TBD |

## Data and security considerations
Document data categories, ownership, storage, retention, access controls, and flows. Never place secrets or real sensitive user data in this document.

## Decisions and alternatives
For each major decision, record a stable decision ID, linked requirement IDs, options considered, evidence/source date, trade-offs, decision owner/approver, lifecycle state, and review trigger. Keep unresolved decisions marked OPEN. Do not claim an architecture decision is approved unless approval evidence exists.

## Key flows and deployment boundaries
- Request/data flow and trust boundaries: TBD.
- Persistent data stores, retention, and deletion paths: TBD.
- Identity/authentication and server-side authorization boundaries: TBD where applicable.
- Runtime/deployment environments and configuration boundaries: TBD.
- Observability, failure containment, rollback, and recovery: TBD.

## Acceptance criteria
- [ ] System boundaries and major components are understandable.
- [ ] Data flows and trust boundaries are identified.
- [ ] External dependencies and failure modes are documented.
- [ ] Important decisions include rationale and alternatives.
- [ ] Architecture is reviewed against approved requirement IDs before implementation.
- [ ] Components, data flows, trust boundaries, external calls, and failure/recovery paths are identified where applicable.
- [ ] Material decisions link to evidence and approval records; open decisions remain explicitly open.

## Dependencies
Project Discovery, Requirements, Section 01 product boundaries.

## Next action
Create the project-specific architecture only after discovery and requirements are reviewed.
