# Dependency Policy

**Status:** 🔴 RED — dependency policy template only; no project inventory has been audited here.

## Selection and maintenance rules
- Add a dependency only for a defined need; consider a smaller native alternative first.
- Review maintenance activity, supported versions, license, provenance, security history, and transitive dependencies as applicable.
- Pin or constrain versions using the project's package manager and commit the appropriate lockfile where applicable.
- Prefer reproducible installs and automated checks; document exceptions.
- Review update impact and run relevant tests before merging upgrades.
- Remove unused dependencies when safe and supported by evidence; do not perform destructive cleanup without review.
- Keep credentials out of manifests, lockfiles, source, and logs.

## Minimum evidence for each material dependency
Record the official project/package URL, exact resolved version, release notes or advisory checked date, license evidence, provenance/source, maintenance/support status, transitive impact, data/network permissions where relevant, and the reason the dependency is needed. If a field is not applicable, record why rather than leaving an ambiguous blank. Use the actual package manager and repository evidence; do not assume every ecosystem supports the same lockfile or audit command.

## Inventory and risk register
| Package / service | Direct or transitive | Version | Purpose | License / support evidence | Security / maintenance risk | Owner / action |
|---|---|---|---|---|---|---|
| TBD | TBD | TBD | TBD | TBD | TBD | TBD |

## Exception and remediation controls
For a vulnerability, abandoned package, incompatible license, or unverifiable provenance, record severity/impact, affected versions, exploitability/context, owner, mitigation, target date, acceptance authority if temporary risk is retained, and re-check/expiry trigger. A clean automated audit does not prove that all supply-chain risks are absent.

## Update process
1. Identify update and reason.
2. Review release notes, compatibility, and relevant advisories.
3. Update in a focused change and inspect lockfile diff.
4. Run install, build, type, unit/integration, and regression checks as applicable.
5. Record result, unresolved findings, and rollback plan for high-impact updates.

## Acceptance criteria
- [ ] Actual dependencies are inventoried for the target project.
- [ ] Selection and update criteria are applied consistently.
- [ ] Vulnerabilities and unsupported packages have tracked actions.
- [ ] Reproducibility and lockfile policy are explicit.
- [ ] Changes are verified and documented; no blanket security claim is inferred.
