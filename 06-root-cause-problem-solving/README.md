# Section 06 — Root-Cause Problem Solving

**Status:** 🔴 RED — structure only; substantive work pending.

## Purpose
Use evidence-led diagnosis and a bounded investigation protocol to solve problems at their source.

## Planned documents
- INCIDENT-INTAKE.md — symptoms, impact, reproduction, and environment.
- DIAGNOSTIC-PROTOCOL.md — hypotheses and evidence collection.
- THREE-ATTEMPT-RULE.md — distinct attempts, stopping conditions, and escalation.
- RESEARCH-PROTOCOL.md — official docs, issue trackers, release notes, and alternatives.
- ROOT-CAUSE-REPORT.md — cause, evidence, fix, and residual risk.
- ACCEPTANCE-CRITERIA.md — evidence required to complete this section.
- STATUS.md — current state and next action.

## Dependencies
Uses the testing and evidence rules in Sections 09–10.
## Evidence and record integrity
Use a stable incident/diagnostic ID and preserve links between intake, hypothesis/test records, research notes, changes, regression results, and the root-cause report. Record timestamp and time zone, environment, baseline commit/version, evidence source, owner, and review state. Separate observations from inference and confirmed cause from provisional explanation.

## Guardrail
Do not repeat equivalent attempts after failure without new evidence or a materially different hypothesis. Stop earlier when safety, security, privacy, destructive risk, or missing authorization requires it.
