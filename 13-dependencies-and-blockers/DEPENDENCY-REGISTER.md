# Dependency Register

**Status:** 🔴 RED — register template; project-specific inventory pending.

## Required fields
- Dependency ID and name.
- Type: internal section, package, runtime, provider/API, infrastructure, credential/configuration, or decision.
- Consumer and purpose.
- Owner and maintainer.
- Required version/capability and compatibility constraints.
- Criticality and failure impact.
- Availability/support assumptions and evidence.
- Status, blocker, fallback, and next review date.

## Rules
Record direct and material transitive dependencies. Distinguish mandatory from optional dependencies and document what capability fails if each is unavailable. Avoid recording secret values; reference the approved secret location or configuration key only.

## Dependencies
Sections 02–03, 09–11, and 14–17.

## Acceptance evidence
A real project inventory covers all critical dependencies and identifies owners, compatibility, and failure impact.

## Next action
Populate from the actual architecture and dependency manifests.
