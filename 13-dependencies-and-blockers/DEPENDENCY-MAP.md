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
|---|---|---|---|---|---|
| EDGE-001 | 01 → 02 | BLOCKING PREREQUISITE | Approved problem, users, goals, scope, and explicit account/identity disposition are required before project-specific planning is baselined. | TBD / approved scope and requirement baseline | Proposed |
| EDGE-002 | 01–02 → 03 | BLOCKING PREREQUISITE | Technology choices must map to approved requirements, product goals, and constraints. | TBD / approved requirements and standards decision records | Proposed |
| EDGE-003 | 01–03 → 04 | BLOCKING PREREQUISITE | The structure-phase blueprint must reflect approved scope, plan, and engineering constraints before project implementation starts. | TBD / approved structure blueprint and gate record | Proposed |
| EDGE-004 | 05 → approval-gated actions across all sections | CROSS-CUTTING CONTROL | Required human approval must be obtained before the specific approval-gated action; numeric order and GREEN status never substitute for consent. | TBD / approval record tied to action ID | Proposed |
| EDGE-005 | 11 → security/privacy-sensitive work and release | CROSS-CUTTING CONTROL | Applicable security, privacy, access-control, and secret-handling gates must pass before affected operations or release. | TBD / scoped threat-control-test evidence | Proposed |
| EDGE-006 | 09 → 06, 07, 10, 11, 17 | COORDINATION / REFERENCE | Apply evidence and source-quality rules where relevant; Section 09 need not be fully GREEN before diagnosis can begin. | TBD / source and evidence records | Proposed |
| EDGE-007 | 10 → GREEN/LOCKED and release gates | BLOCKING PREREQUISITE | Required verification evidence must exist for the specific acceptance/release decision; the whole Section 10 need not be GREEN if the gate has separately approved evidence requirements. | TBD / test IDs and acceptance evidence | Proposed |
| EDGE-008 | 06 → 07 | COORDINATION / REFERENCE | Root-cause findings inform repair review; Section 07 is not a blanket prerequisite for diagnosis. | TBD / diagnosis and change records | Proposed |
| EDGE-009 | 14 → 07, 17 | COORDINATION / REFERENCE; sometimes BLOCKING | Maintenance, migration, compatibility, and rollback knowledge informs fixes/releases; an applicable migration or recovery gate blocks only the affected change. | TBD / component lifecycle and recovery evidence | Proposed |
| EDGE-010 | 13 → 02, 04, 14, 17 | COORDINATION / REFERENCE; sometimes BLOCKING | Dependency/blocker records inform planning; a critical unresolved blocker blocks only activities/releases within its recorded impact. | TBD / blocker ID, impact, owner, and clearing evidence | Proposed |
| EDGE-011 | 12 → all status transitions | CROSS-CUTTING CONTROL | Status labels and transitions follow one evidence-based rule and cannot override approval, security, or release controls. | TBD / transition scenario evidence | Proposed |
| EDGE-012 | 15 → material decisions, evidence, status changes, and handoffs | CROSS-CUTTING CONTROL | Durable records and handoffs must be traceable in the agreed source of truth; this does not require every Section 15 document to be GREEN before work. | TBD / linked decision and handoff records | Proposed |
| EDGE-013 | 16 → review and collaboration workflows | COORDINATION / REFERENCE | Responsibilities identify who performs/reviews work but do not independently grant approval authority. | TBD / role-to-authority map and review scenario | Proposed |
| EDGE-014 | Approved Section 18 baseline → work governed by this methodology | BLOCKING PREREQUISITE (baseline only) | The applicable working agreement and approval boundaries must be reconciled and approved before the method baseline is treated as authoritative; this does not prevent safe review of the draft method itself. | TBD / owner-approved agreement/version record | Proposed; owner approval pending |
| EDGE-015 | 15, 16, 17 → Section 18 method evolution | DOWNSTREAM CONSUMER | Handoffs, reviews, and release outcomes supply later lessons/evolution evidence; completing Sections 15–17 is not a prerequisite for drafting Section 18. | TBD / lesson IDs and approved evolution proposal | Proposed |
| EDGE-016 | Section 18 approved baseline → 15, 16, 17 | COORDINATION / REFERENCE (full section) | The approved agreement/versioning baseline governs relevant work; future lessons/evolution activities are not a blanket blocker for documentation, collaboration, or release. | TBD / approved baseline and applicability record | Proposed |
| EDGE-017 | 01 → substantive project implementation | BLOCKING PREREQUISITE | Approved purpose, target users, value, and scope are required before project-specific implementation is baselined; structural methodology review is not blocked. | TBD / approved scope and requirement baseline | Proposed |
| EDGE-018 | 08 → all active work/handoffs when pause triggers apply | CROSS-CUTTING CONTROL | Stop-work, checkpoint, and resume rules apply when triggered; Section 08 need not be GREEN before unrelated safe work can proceed. | TBD / pause-resume scenario evidence | Proposed |
| EDGE-019 | 11 → security/privacy-sensitive work | CROSS-CUTTING CONTROL | Applicable security, privacy, access, secret-handling, and fail-closed controls apply before affected operations; scope depends on data flow and threat. | TBD / threat-control-test evidence | Proposed |
| EDGE-020 | 01–03, 05–09, 11 → 10 | COORDINATION / REFERENCE | Test strategy consumes approved requirements, engineering/security constraints, diagnostic/research evidence, and privacy/security controls; apply only criteria relevant to the tested scope. | TBD / requirement-risk-to-test map | Proposed |
| EDGE-021 | 03, 06–07, 09–11, 13 → 14 | COORDINATION / REFERENCE | Maintenance uses lifecycle standards, incident/patch history, test evidence, security/privacy requirements, and dependency records; a specific migration/recovery gate may block the affected change. | TBD / lifecycle and operations evidence | Proposed |
| EDGE-022 | Applicable outputs from 01–16 and approved Section 18 baseline → 17 | DOWNSTREAM CONSUMER; sometimes BLOCKING | Release review consumes applicable scope, approval, test, security, operations, recovery, support, and governance evidence. Only an applicable release-critical criterion blocks release; an entire upstream section need not be GREEN by default. | TBD / release evidence matrix and GO/NO-GO record | Proposed |
| EDGE-023 | 05, 09–10, 12, 15–17 → Section 18 lessons/evolution | DOWNSTREAM CONSUMER | Methodology lessons and evolution proposals consume approval, research, test, status, continuity, collaboration, and release outcomes; these are inputs to proposed improvements, not prerequisites for the existing approved baseline. | TBD / lesson IDs, evidence, and approved evolution proposal | Proposed |
| EDGE-024 | 05, 09–13, 15, 17–18 → 16 | COORDINATION / REFERENCE | Roles, reviews, communications, and disputes align with approval, evidence, status, dependency, continuity, release, and agreement rules; role assignment never grants authority. | TBD / role-to-authority and review scenario evidence | Proposed |
| EDGE-025 | 01 → architecture, scope, security, testing, and release decisions across the method | COORDINATION / REFERENCE | Section 01 is a source of product purpose, users, value, scope, and account/identity disposition; downstream sections reference approved outputs rather than requiring Section 01 to be wholly GREEN for structural review. | TBD / requirement and decision traceability | Proposed |
| EDGE-026 | 01–02 → 05 | COORDINATION / REFERENCE | Approval and autonomy boundaries use approved scope and risk context; approval policy cannot authorize work outside the approved scope. | TBD / scope-to-approval matrix | Proposed |
| EDGE-027 | 09–10 → 06 | COORDINATION / REFERENCE | Diagnosis uses available evidence and test results; absence of evidence is recorded as uncertainty, not treated as proof. This edge is non-blocking to initial triage. | TBD / diagnosis record linked to evidence/test IDs | Proposed |
| EDGE-028 | 06, 09, 10, 14 → 07 | COORDINATION / REFERENCE | Patch prevention uses root-cause findings, research quality, regression tests, and maintenance/rollback constraints; applicable regression/recovery evidence may block a specific patch. | TBD / change risk and regression evidence | Proposed |
| EDGE-029 | 01–02, 03 → 10 | COORDINATION / REFERENCE | Acceptance criteria and tests derive from approved scope/requirements and applicable engineering standards; missing critical acceptance criteria block the affected acceptance decision. | TBD / requirement-to-test traceability | Proposed |
| EDGE-030 | 03, 13 → 14 | COORDINATION / REFERENCE | Maintenance/update decisions use technology lifecycle standards and recorded internal/external dependency ownership, versions, and criticality. | TBD / dependency inventory and lifecycle evidence | Proposed |
| EDGE-031 | 05, 09–14, 17–18 → 15 | CROSS-CUTTING CONTROL / COORDINATION | Continuity records handoffs, decisions, evidence, maintenance/security outcomes, release events, and applicable agreement versions. It creates traceability requirements, not a blanket sequence blocker. | TBD / handoff and change-history evidence | Proposed |
| EDGE-032 | 05, 09–13, 15, 17–18 → 16 | COORDINATION / REFERENCE | Collaboration and review workflows must align with authority, evidence, status, blocker, continuity, release, and approved-agreement rules. | TBD / role-to-authority and review/dispute scenario | Proposed |
| EDGE-033 | 12, 15, 16, 17 → governed status, collaboration, and release records | COORDINATION / REFERENCE | The approved agreement must be reflected in status, durable records, role boundaries, and release decisions; no draft policy silently overrides existing approved controls. | TBD / cross-section governance scenario | Proposed |
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
