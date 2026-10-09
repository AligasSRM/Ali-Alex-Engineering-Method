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

| Source → consumer | Type | Boundary / rule | Validation state |
|---|---|---|---|
| 01 → 02 | BLOCKING PREREQUISITE | Approved problem, users, goals, scope, and explicit account/identity disposition are required before project-specific planning is baselined. | Proposed |
| 02 → 03 | BLOCKING PREREQUISITE | Technology choices must map to approved requirements and constraints. | Proposed |
| 01–03 → 04 | BLOCKING PREREQUISITE | The structure-phase blueprint must reflect the approved scope, plan, and engineering constraints before implementation starts. | Proposed |
| 05 → all sections | CROSS-CUTTING CONTROL | Required human approval must be obtained before any approval-gated action; numeric order and GREEN status never substitute for consent. | Proposed |
| 11 → security-sensitive work and release | CROSS-CUTTING CONTROL | Applicable security, privacy, access-control, and secret-handling gates must pass before affected work proceeds or is released. | Proposed |
| 09 → 06, 07, 10, 11, 17 | COORDINATION / REFERENCE | Use evidence and source-quality rules where applicable; these references do not require Section 09 to be fully GREEN before a diagnosis can start. | Proposed |
| 10 → GREEN/LOCKED and release gates | BLOCKING PREREQUISITE | Required verification evidence must exist for the specific acceptance or release decision. The entire Section 10 need not be GREEN if the relevant gate has independently defined, approved evidence requirements. | Proposed |
| 06 → 07 | COORDINATION / REFERENCE | Root-cause findings inform repair review; a diagnosis workflow may reference Section 07 without making all of Section 07 a prerequisite. | Proposed |
| 14 → 07, 17 | COORDINATION / REFERENCE | Maintenance, migration, compatibility, and rollback knowledge informs fixes and releases. A relevant migration/recovery gate may become blocking for that change. | Proposed |
| 13 → 02, 04, 14, 17 | COORDINATION / REFERENCE; sometimes BLOCKING | Dependency and blocker records inform planning. Any unresolved critical blocker is blocking only when its recorded impact affects the current activity or release. | Proposed |
| 12 → all status transitions | CROSS-CUTTING CONTROL | Status labels and transitions must follow one evidence-based rule. A status label cannot override approval, security, or release controls. | Proposed |
| 15 → all handoffs and durable records | CROSS-CUTTING CONTROL | Material decisions, evidence, status changes, and handoffs must be traceable in the agreed source of truth. | Proposed |
| 16 → review and collaboration workflows | COORDINATION / REFERENCE | Responsibilities identify who does/reviews work; they do not independently grant approval authority. | Proposed |
| 18 baseline agreement → work under the methodology | BLOCKING PREREQUISITE (baseline only) | The applicable working-agreement and approval boundaries must be reconciled and approved before the method baseline is treated as authoritative. | Proposed; owner approval pending |
| 15, 16, 17 → 18 method evolution | DOWNSTREAM CONSUMER | Handoffs, reviews, and release outcomes supply lessons and evidence for later method evolution; full completion of Sections 15–17 must not be a circular prerequisite for drafting Section 18. | Proposed |
| 18 → 15, 16, 17 | COORDINATION / REFERENCE (full section) | Section 18 provides agreement/versioning rules. Its future lessons-learned and evolution workflow is not a blocking prerequisite for every documentation, collaboration, or release activity. | Proposed |

## Rules for cycles and sequence

1. Do not treat all cross-references as blocking dependencies.
2. A blocking edge must name the exact deliverable or control required, the activity/gate it blocks, and the evidence that clears it.
3. If A and B appear to block each other, split baseline controls from later maturity work or redesign the edge; do not silently ignore the cycle.
4. Approval, security/privacy, required acceptance evidence, and release controls take precedence over section order, role titles, convenience, and status colors.
5. A deferral never removes a mandatory safety/security/approval gate; it must record risk, authority, and re-entry conditions.
6. Any changed edge must be reflected in this map, the source and consumer documents, and the audit report.

## Explicit unresolved decisions

- Confirm the exact minimum approved Section 18 baseline needed before Section 01 work.
- Validate the Section 15 project-history vs Section 18 methodology-versioning boundary.
- Define one Section 12 reopening path and one precedence rule across Sections 05, 11, 12, and 17.
- Decide whether operational observability (logs, metrics, alerts, service objectives, incident escalation/runbooks) is adequately owned by Sections 06, 14, and 17 or needs a distinct section. Do not add a new numbered section until this gap is checked against the full document set.
- Reconcile this proposed map with every section README, dependency declaration, acceptance criterion, and status record.

## Acceptance

This map remains RED until every declared edge is checked against source documents, blocking edges are acyclic or explicitly justified, the owner approves the governance decisions, and the audit records verification evidence. This draft is not proof of completed compatibility.
