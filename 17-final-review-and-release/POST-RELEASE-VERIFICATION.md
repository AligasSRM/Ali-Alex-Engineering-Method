# Post-Release Verification

**Status:** RED — verification plan drafted; release observation not performed.

## Verification run metadata
- Release ID / verification run ID:
- Exact deployed commit/artifact identity and environment:
- Observation window start/end and time zone:
- Health indicators, approved thresholds, data sources, and owners:
- Evidence IDs/artifacts and last-checked time:

## Verify after release
- [ ] The deployed version matches the approved commit/build artifact.
- [ ] Critical user journeys and service health checks pass.
- [ ] Authentication, authorization, and safety gates behave as expected.
- [ ] Data integrity and critical business transactions reconcile.
- [ ] Error rates, latency, saturation, and relevant business indicators remain within approved thresholds.
- [ ] Alerts, logs, and audit records are available without exposing sensitive data.
- [ ] External integrations and callbacks behave as expected.
- [ ] No unexpected cost, quota, or resource spike is observed.
- [ ] Support/incident ownership is active and escalation paths work.
- [ ] Release decision and observed results are recorded.

## Failure response
A failed, missing, or inconclusive critical check prevents a claim of successful release verification. Record the affected scope, whether containment/rollback is required, decision owner, and re-verification criteria.

## Failure response
Use the approved containment and recovery plan. Do not broaden scope during an incident without the appropriate authority. If required verification cannot be performed, report the gap and follow the release policy rather than claiming success.

## Dependencies
Sections 09–14, 16, and the release decision in this section.

## Acceptance evidence
Recorded observations are tied to the exact deployment and the defined observation window.

## Next action
Define project-specific health indicators and a safe post-release observation window.
