# Dependency Register

**Status:** 🔴 RED — register template only; dependencies have not been inventoried.

| ID | Dependency / service / team | Internal or external | Purpose | Owner | Version / contract | Availability / risk | Fallback / mitigation | Evidence |
|---|---|---|---|---|---|---|---|---|
| DEP-001 | TBD | TBD | TBD | TBD | TBD | TBD | TBD | TBD |

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

## Next action
Populate from the current-state audit and proposed architecture.
