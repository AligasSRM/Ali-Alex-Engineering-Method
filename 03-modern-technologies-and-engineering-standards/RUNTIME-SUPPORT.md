# Runtime Support Policy

**Status:** 🔴 RED — policy template only; supported versions depend on each project's requirements.

## Runtime inventory
| Runtime / tool | Required version range / pin | Official lifecycle URL + version | Date checked | End-of-support date / status | OS / framework / package-manager compatibility evidence | Upgrade / rollback path | Owner / review trigger |
|---|---|---|---|---|---|
| TBD | TBD | TBD | TBD | TBD | TBD | TBD | TBD |

## Policy
- Record exact runtime, framework, package-manager, and build-tool versions where relevant.
- Use official lifecycle/support sources and record when they were checked.
- Avoid unsupported or end-of-life versions unless a documented exception and containment plan are approved.
- Plan upgrades with compatibility checks, tests, rollback strategy, and dependency review.
- Do not infer production support from a successful local install.

## Compatibility gate
Check the complete supported combination (operating system, runtime, framework, package manager, build/test tools, deployment target, and native dependencies where relevant). Record tested versions and environment; do not infer compatibility from a version range alone. Pin versions in the repository's supported mechanism where reproducibility requires it, and define how pins are refreshed.

## Exception record
- Component/version: TBD
- Reason and impact: TBD
- Mitigation and target resolution date: TBD
- Approver: TBD

## Acceptance criteria
- [ ] Applicable runtimes and tools are inventoried.
- [ ] Support status is backed by dated official evidence.
- [ ] Upgrade/exception handling is documented.
- [ ] Project owner reviews the policy against actual constraints.
