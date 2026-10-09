# Incident Intake

**Status:** 🔴 RED — template drafted; not validated on a real incident.

## Purpose
Capture a reproducible, evidence-based description before diagnosing a problem.

## Intake record
- Project/repository and affected component:
- Date/time and environment/version:
- Expected behavior:
- Actual behavior and exact error/output:
- Reproduction steps and frequency:
- Scope and user/business impact:
- Recent changes and last known-good state:
- Logs, screenshots, test output, and source references:
- Known constraints and safety boundaries:
- Immediate containment already authorized:
- Unknowns and missing evidence:

## Rules
Separate observed facts from interpretation. Redact secrets and unnecessary personal data from evidence. Do not make destructive changes merely to improve reproduction. If impact or authorization is unclear, use Section 05 escalation and approval controls.

## Dependencies
Section 02 current-state audit; Section 05 escalation; Section 09 evidence standards; Section 10 testing.

## Acceptance evidence
A second engineer can understand the symptom and reproduce it, or see exactly why reproduction is currently blocked.

## Next action
Use this template on a real incident and review it against the diagnostic protocol.
