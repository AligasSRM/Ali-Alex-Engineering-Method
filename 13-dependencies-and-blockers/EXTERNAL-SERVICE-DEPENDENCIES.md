# External Service Dependencies

**Status:** 🔴 RED — inventory guidance drafted; provider inventory pending.

## Record for each provider
- Stable service/dependency ID, status, owner, and affected capability/requirement IDs:
- Service and business purpose.
- Official documentation/status page URL, API/SDK version, date checked, and captured status evidence.
- API/SDK version and compatibility requirements.
- Authentication method, stored separately from the record.
- Data sent/received and privacy implications.
- Rate limits, quotas, cost exposure, and billing triggers.
- Availability/SLA assumptions with source/version/date, observed limitations, and the exact scope covered.
- Timeout, retry, idempotency, rate-limit, partial-failure, and outage behavior; tested versus assumed behavior.
- Sandbox versus live environment distinction.
- Alternative, degradation mode, or recovery plan.
- Owner and last verification date.

## Controls
Record data categories sent/received, data residency/cross-border considerations, access scope, billing/renewal triggers, and account ownership. Identify the safe degradation mode and the capability that must stop if the provider is unavailable.
Verify current details from authoritative provider sources. Do not assume a free tier, availability, or API behavior without evidence. External calls, account changes, charges, and live activation require the approvals applicable to the action.

## Dependencies
Sections 03, 05, 09–11, and 14–17.

## Acceptance evidence
Critical external dependencies have documented operational, security, privacy, and cost assumptions.

## Next action
Inspect actual integration points and verify provider-specific facts.
