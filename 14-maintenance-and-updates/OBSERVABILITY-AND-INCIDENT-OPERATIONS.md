# Observability and Incident Operations

**Status:** 🔴 RED — scope and controls drafted; project-specific design and exercise pending.

## Purpose

Define how a deployed system's health is observed, how abnormal behavior is detected, and how incidents are triaged, escalated, contained, and learned from. This document complements Section 06's root-cause diagnosis, Section 11's security/privacy controls, and Section 17's release readiness and post-release verification.

## Minimum operational signals

For each production-critical service or workflow, identify applicable signals and record why any signal is not relevant:

- **Availability and correctness:** health checks, critical user journeys, job/transaction success, data integrity, and dependency reachability.
- **Latency and capacity:** response/job duration, queue depth, saturation, resource limits, and rate limits where relevant.
- **Failures:** error rates, retries, timeouts, failed callbacks, dead-letter/backlog indicators, and dependency failures.
- **Business/service objectives:** measurable service-level indicators and objectives appropriate to the product's risk and scale; do not invent targets without an owner-approved basis.
- **Security and audit:** authentication/authorization failures, privileged actions, suspicious abuse patterns, and required audit events, with privacy-aware handling.
- **Cost and quotas:** material usage, spend, quota exhaustion, and unusual resource growth where cost exposure exists.

## Logging and alerting rules

- Logs must support diagnosis without recording passwords, access tokens, private keys, or unnecessary personal data.
- Where traces or correlation identifiers are used, avoid embedding sensitive payloads in them.
- Each actionable alert must have a severity, trigger, owner/on-call or escalation path, first-response steps, and a way to determine whether the alert is resolved.
- Alerts should be actionable and risk-based; noisy or unactionable alerts must be reviewed rather than ignored.
- Define retention, access, redaction, and integrity controls for operational and audit records under Section 11.
- Record monitoring blind spots, unavailable telemetry, and provider limitations explicitly.

## Incident operations

1. Detect or receive a report and record time, affected service, scope, and evidence.
2. Assess impact and severity using project-specific criteria.
3. Apply only pre-authorized containment; obtain Section 05 approval for high-impact or ambiguous actions.
4. Assign an incident owner and communicate verified facts, uncertainty, user impact, and next update.
5. Preserve evidence safely and follow Section 06's diagnostic protocol without delaying necessary containment.
6. Recover through an approved rollback, failover, or repair path; verify actual service recovery.
7. Record timeline, cause confidence, residual risk, customer impact, and follow-up actions.
8. Review recurring causes and feed approved lessons into Sections 14, 15, and 18.

## Required per-project record

For each critical service/workflow, document: owner, critical user journeys, health signals, thresholds and their rationale, dashboards/queries, alert routes, response runbook, escalation authority, log/telemetry retention, privacy controls, known blind spots, recovery procedure, and review cadence.

## Acceptance evidence

- [ ] Critical services/workflows and operational owners are identified.
- [ ] Health signals and thresholds have an evidence-based rationale and approval.
- [ ] Alerts route to a responsible owner and include actionable response steps.
- [ ] Telemetry is tested while avoiding secrets and unnecessary personal data.
- [ ] A representative alert/incident exercise demonstrates detection, escalation, containment, recovery, and evidence capture.
- [ ] Post-recovery verification is tied to the actual service state.
- [ ] Gaps, residual risks, and follow-up owners are recorded.

## Dependencies

Sections 05, 06, 09–11, 13, 15, and 17. Section 17 remains the release gate; this document defines ongoing operational ownership and monitoring after deployment.

## Guardrail

Do not claim production monitoring or incident readiness from a checklist alone. Require project-specific configuration and an observed exercise before marking the relevant criteria GREEN.
