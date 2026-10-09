# Dependency Register

**Status:** 🔴 RED — register template only; dependencies have not been inventoried.

| ID | Dependency / service / team | Internal or external | Purpose / linked requirement IDs | Owner | Version / contract | Criticality / availability risk | Fallback / fail behavior | Evidence / last checked |
|---|---|---|---|---|---|---|---|---|
| DEP-001 | TBD | TBD | TBD | TBD | TBD | TBD | TBD | TBD |

## Ownership and synchronization
This file captures dependencies discovered during project planning. Section 13 owns the cross-method dependency/blocker map, escalation, and deferred-work status. Keep stable dependency IDs across both records; link rather than copy detailed status. Any critical unresolved dependency must appear in the Section 13 blocker register before a plan is approved.

## Dependency rules
- Identify runtime, build, test, deployment, data, identity, and third-party service dependencies.
- Record version constraints and license/compliance considerations when applicable.
- Distinguish required dependencies from optional enhancements.
- Document credentials by secret-manager reference only; never record secret values.
- State what happens when a dependency is unavailable and how failure is tested.

## Acceptance criteria
- [ ] Each material dependency has purpose and owner.
- [ ] Version/contract and availability risks are recorded where relevant.
- [ ] Critical dependency failures have a mitigation or explicit blocker.
- [ ] Evidence links or the reason evidence is unavailable are recorded.
- [ ] Dependency IDs and critical blockers are synchronized with Section 13; ownership is not duplicated inconsistently.

## Next action
Populate from the current-state audit and proposed architecture.
