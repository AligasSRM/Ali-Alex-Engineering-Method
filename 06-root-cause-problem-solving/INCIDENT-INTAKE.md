# Incident Intake

**Status:** 🔴 RED — template drafted; not validated on a real incident.

## Purpose
Capture a reproducible, evidence-based description before diagnosing a problem.

## Intake record
- Incident ID / linked ticket or blocker ID:
- Reporter / accountable owner / current severity:
- Date/time/time zone and last updated:
- Project/repository and affected component:
- Environment, runtime/tool versions, branch/commit, deployment identifier:
- Expected behavior:
- Actual behavior and exact error/output:
- Reproduction steps and frequency:
- Scope and user/business impact:
- Recent changes and last known-good state:
- Evidence inventory (source, timestamp, integrity/location, what it proves):
- Known constraints and safety boundaries:
- Immediate containment already authorized (approval ID/scope, if applicable):
- Unknowns and missing evidence:

## Handling and evidence rules
- Use the project's approved severity and incident-response scheme; do not invent severity labels or response-time commitments.
- Preserve original evidence where feasible and record any redaction, transformation, or unavailable source. Avoid collecting secrets or unnecessary personal data.
- Record the command/query and environment needed to reproduce evidence, while keeping credentials and sensitive values out of the report.

## Rules
Separate observed facts from interpretation. Redact secrets and unnecessary personal data from evidence. Do not make destructive changes merely to improve reproduction. If impact or authorization is unclear, use Section 05 escalation and approval controls.

## Dependencies
Section 02 current-state audit; Section 05 escalation; Section 09 evidence standards; Section 10 testing.

## Acceptance evidence
A second engineer can understand the symptom and reproduce it, or see exactly why reproduction is currently blocked.

## Next action
Use this template on a real incident and review it against the diagnostic protocol.
