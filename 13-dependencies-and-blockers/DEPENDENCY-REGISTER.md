# Dependency Register

**Status:** 🔴 RED — register template; project-specific inventory pending.

## Required fields
- Stable dependency ID and record state: PROPOSED / VERIFIED / DEGRADED / BLOCKED / RETIRED.
- Dependency ID and name.
- Type: internal section, package, runtime, provider/API, infrastructure, credential/configuration, or decision.
- Consumer and purpose; linked requirement/architecture/edge IDs.
- Owner and maintainer.
- Required version/capability and compatibility constraints.
- Criticality and failure impact.
- Official source URL, version/capability, date checked, compatibility evidence, and support/availability assumptions.
- Failure behavior, fallback/recovery owner, linked blocker/risk IDs, evidence, last-reviewed timestamp/time zone, and next review trigger/date.

## Rules
Record direct and material transitive dependencies. Distinguish mandatory from optional dependencies and document what capability fails if each is unavailable. Avoid recording secret values; reference the approved secret location or configuration key only.

## Dependencies
Sections 02–03, 09–11, and 14–17.

## Lifecycle rules
A dependency is VERIFIED only when the required capability/version and relevant environment have been checked. If the provider changes version, terms, availability, authentication, or data handling, revalidate affected consumers. Never treat a documented fallback as tested until evidence exists.

## Acceptance evidence
A real project inventory covers all critical dependencies and identifies owners, compatibility, and failure impact.

## Next action
Populate from the actual architecture and dependency manifests.
