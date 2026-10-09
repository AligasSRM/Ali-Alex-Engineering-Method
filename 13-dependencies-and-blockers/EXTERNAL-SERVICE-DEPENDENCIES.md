# External Service Dependencies

**Status:** 🔴 RED — inventory guidance drafted; provider inventory pending.

## Record for each provider
- Service and business purpose.
- Official documentation and status page.
- API/SDK version and compatibility requirements.
- Authentication method, stored separately from the record.
- Data sent/received and privacy implications.
- Rate limits, quotas, cost exposure, and billing triggers.
- Availability/SLA assumptions and observed limitations.
- Timeout, retry, idempotency, and outage behavior.
- Sandbox versus live environment distinction.
- Alternative, degradation mode, or recovery plan.
- Owner and last verification date.

## Controls
Verify current details from authoritative provider sources. Do not assume a free tier, availability, or API behavior without evidence. External calls, account changes, charges, and live activation require the approvals applicable to the action.

## Dependencies
Sections 03, 05, 09–11, and 14–17.

## Acceptance evidence
Critical external dependencies have documented operational, security, privacy, and cost assumptions.

## Next action
Inspect actual integration points and verify provider-specific facts.
