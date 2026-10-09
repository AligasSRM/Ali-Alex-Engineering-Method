# Cross-Section Dependency Map — Initial Classification

**Status:** 🔴 RED — initial classification for review; not yet owner-approved or validated against every document.

## Purpose and direction

This file is the shared map for dependencies among methodology sections. An edge written as **A → B** means **B consumes, follows, or is governed by output from A**. The edge type determines whether B must wait for A to be complete.

- **BLOCKING PREREQUISITE:** the named output/control must be verified before the specified activity or gate can proceed.
- **COORDINATION / REFERENCE:** consult the source when relevant; it does not force the entire source section to be completed first.
- **DOWNSTREAM CONSUMER:** the consumer uses the source output later; this is not a prerequisite for building the source.
- **CROSS-CUTTING CONTROL:** applies wherever its trigger is present, regardless of the numeric section order.

A reference to a later-numbered section is not automatically a sequencing error. Only a dependency explicitly classified as blocking can stop a gate.

## Initial dependency classifications

| Edge ID | Source → consumer | Type | Boundary / exact output or gate | Owner / clearing evidence | Validation state |
|---|---|---|---|
| EDGE-001 | 01 → 02 | BLOCKING PREREQUISITE | Approved problem, users, goals, scope, and explicit account/identity disposition are required before project-specific planning is baselined. | TBD / TBD | Proposed |
| EDGE-002 | 02 → 03 | BLOCKING PREREQUISITE | Technology choices must map to approved requirements and constraints. | TBD / TBD | Proposed |
| EDGE-003 | 01–03 → 04 | BLOCKING PREREQUISITE | The structure-phase blueprint must reflect the approved scope, plan, and engineering constraints before implementation starts. | TBD / TBD | Proposed |
| EDGE-004 | 05 → all sections | CROSS-CUTTING CONTROL | Required human approval must be obtained before any approval-gated action; numeric order and GREEN status never substitute for consent. | TBD / TBD | Proposed |
| EDGE-005 | 11 → security-sensitive work and release | CROSS-CUTTING CONTROL | Applicable security, privacy, access-control, and secret-handling gates must pass before affected work proceeds or is released. | TBD / TBD | Proposed |
| EDGE-006 | 09 → 06, 07, 10, 11, 17 | COORDINATION / REFERENCE | Use evidence and source-quality rules where applicable; these references do not require Section 09 to be fully GREEN before a diagnosis can start. | TBD / TBD | Proposed |
| EDGE-007 | 10 → GREEN/LOCKED and release gates | BLOCKING PREREQUISITE | Required verification evidence must exist for the specific acceptance or release decision. The entire Section 10 need not be GREEN if the relevant gate has independently defined, approved evidence requirements. | TBD / TBD | Proposed |
| EDGE-008 | 06 → 07 | COORDINATION / REFERENCE | Root-cause findings inform repair review; a diagnosis workflow may reference Section 07 without making all of Section 07 a prerequisite. | TBD / TBD | Proposed |
| EDGE-009 | 14 → 07, 17 | COORDINATION / REFERENCE | Maintenance, migration, compatibility, and rollback knowledge informs fixes and releases. A relevant migration/recovery gate may become blocking for that change. | TBD / TBD | Proposed |
| EDGE-010 | 13 → 02, 04, 14, 17 | COORDINATION / REFERENCE; sometimes BLOCKING | Dependency and blocker records inform planning. Any unresolved critical blocker is blocking only when its recorded impact affects the current activity or release. | TBD / TBD | Proposed |
| EDGE-011 | 12 → all status transitions | CROSS-CUTTING CONTROL | Status labels and transitions must follow one evidence-based rule. A status label cannot override approval, security, or release controls. | TBD / TBD | Proposed |
| EDGE-012 | 15 → all handoffs and durable records | CROSS-CUTTING CONTROL | Material decisions, evidence, status changes, and handoffs must be traceable in the agreed source of truth. | TBD / TBD | Proposed |
| EDGE-013 | 16 → review and collaboration workflows | COORDINATION / REFERENCE | Responsibilities identify who does/reviews work; they do not independently grant approval authority. | TBD / TBD | Proposed |
| EDGE-014 | 18 baseline agreement → work under the methodology | BLOCKING PREREQUISITE (baseline only) | The applicable working-agreement and approval boundaries must be reconciled and approved before the method baseline is treated as authoritative. | TBD / TBD | Proposed; owner approval pending |
| EDGE-015 | 15, 16, 17 → 18 method evolution | DOWNSTREAM CONSUMER | Handoffs, reviews, and release outcomes supply lessons and evidence for later method evolution; full completion of Sections 15–17 must not be a circular prerequisite for drafting Section 18. | TBD / TBD | Proposed |
| EDGE-016 | 18 → 15, 16, 17 | COORDINATION / REFERENCE (full section) | Section 18 provides agreement/versioning rules. Its future lessons-learned and evolution workflow is not a blocking prerequisite for every documentation, collaboration, or release activity. | TBD / TBD | Proposed |

## Rules for cycles and sequence

1. Do not treat all cross-references as blocking dependencies.
2. A blocking edge must name the exact deliverable or control required, the activity/gate it blocks, and the evidence that clears it.
3. If A and B appear to block each other, split baseline controls from later maturity work or redesign the edge; do not silently ignore the cycle.
4. Approval, security/privacy, required acceptance evidence, and release controls take precedence over section order, role titles, convenience, and status colors.
5. A deferral never removes a mandatory safety/security/approval gate; it must record risk, authority, and re-entry conditions.
6. Any changed edge must be reflected in this map, the source and consumer documents, and the audit report.

## Explicit unresolved decisions

- Confirm the exact minimum approved Section 18 baseline needed before Section 01 work.
- Section 15 owns project/repository history; Section 18 owns methodology/agreement versioning. Cross-links should be used rather than duplicate entries; verify this boundary during the final cross-section pass.
- Section 12 reopening destination rule is now defined in `12-section-status-and-locking/TRANSITION-RULES.md`; final precedence validation across Sections 05, 11, 12, and 17 remains open.
- Current structural decision: operational observability and incident operations are assigned to `14-maintenance-and-updates/OBSERVABILITY-AND-INCIDENT-OPERATIONS.md`, with release gates retained in Section 17, root-cause diagnosis in Section 06, and security/privacy controls in Section 11. No separate Section 19 is justified by this gap at present; revisit only if real-project validation exposes an ownership gap that cannot be assigned cleanly.
- Reconcile this proposed map with every section README, dependency declaration, acceptance criterion, and status record.

## Acceptance

This map remains RED until every declared edge is checked against source documents, blocking edges are acyclic or explicitly justified, the owner approves the governance decisions, and the audit records verification evidence. This draft is not proof of completed compatibility.
