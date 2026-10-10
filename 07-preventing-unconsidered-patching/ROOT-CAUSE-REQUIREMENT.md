# Root-Cause Requirement

**Status:** 🔴 RED — draft; validation pending.

## Purpose
Require sufficient diagnosis before changing code, configuration, data, or operating procedures to address a reported defect.

## Minimum evidence before a fix
- Stable change/patch ID linked to the incident and diagnostic record.
- Repository, branch, baseline commit, relevant versions, and execution environment.
- Explicit status of the causal claim: confirmed, strongly supported, provisional, or unknown.
- Reproducible symptom or a clear account of why reproduction is unavailable.
- Current baseline and affected versions/components.
- At least one supported causal hypothesis, plus known alternatives where uncertainty remains.
- A proposed change linked to the suspected cause.
- Impact scope, side effects, and rollback/recovery plan.
- Targeted tests and regression coverage.
- Required approval under Section 05.

## Temporary mitigation controls
Any temporary mitigation must record the affected users/systems, expected benefit and known side effects, monitoring signal, responsible owner, approval ID where required, expiry/review date, rollback procedure, and the condition that triggers replacement by a permanent fix. Do not silently extend an expired mitigation.

## When the cause is not yet known
Permit bounded, non-destructive diagnostic work. Do not present a speculative workaround as a permanent fix. If a temporary mitigation is needed, label it temporary, define monitoring and expiry/review criteria, and obtain approval when its impact requires it.

## Dependencies
Sections 05–06, 09–10, and 13.

## Acceptance evidence
A reviewer can trace the proposed change to evidence and see why lower-risk alternatives were accepted or rejected.

## Next action
Use this requirement in the patch review checklist and verify the handoff to regression testing.
