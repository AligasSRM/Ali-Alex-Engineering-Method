# Root-Cause Report

**Status:** 🔴 RED — report structure drafted; no incident evidence attached yet.

## Purpose
Record what caused an issue, how the conclusion was established, what changed, and what risk remains.

## Report sections
- **Summary:** concise symptom and impact.
- **Environment and baseline:** versions, relevant configuration, last known-good state.
- **Timeline:** reproduction, diagnostic attempts, and evidence.
- **Root cause:** causal mechanism and confidence level.
- **Evidence:** logs, test output, minimal reproduction, source links, and what each item proves.
- **Contributing factors:** detection gaps, unclear requirements, dependency changes, or missing tests.
- **Resolution:** exact files/configuration/actions changed and why.
- **Verification:** targeted tests, regression tests, and observed outcomes.
- **Rollback:** procedure and prerequisites.
- **Residual risk:** unresolved cases, limitations, and monitoring.
- **Cross-section impact:** affected requirements, standards, status gates, dependencies, and documentation.
- **Decision and next action:** owner/approval if needed, follow-ups, and closure rationale.

## Rules
Do not claim a root cause without supporting evidence. If multiple causes remain plausible, label the result provisional. Never include credentials or unnecessary personal data.

## Dependencies
Sections 05, 07, 09–10, 12–15.

## Acceptance evidence
A real incident report is independently reviewable and links each conclusion to evidence and each fix to verification.

## Next action
Complete the report after a validated real incident and use it to improve preventive controls.
