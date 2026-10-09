# Dependency Updates

**Status:** RED — update policy drafted; dependency inventory and tooling review pending.

## Update classes
- **Critical vulnerability fix:** assess immediately, contain exposure, and prioritize verified remediation.
- **Routine security or bug fix:** evaluate impact and schedule based on risk.
- **Feature/minor update:** review compatibility and value before adoption.
- **Major/breaking update:** plan migration, test dependent interfaces, and define rollback.

## Update record
- Update ID / linked dependency and vulnerability IDs:
- Current and target version / source URL / date checked:
- Baseline commit, manifest/lockfile changes, and affected consumers:
- Change class, severity, compatibility/license/provenance findings:
- Test IDs, exact commands, environment, result, and evidence links:
- Rollback/forward-recovery plan and responsible owner:
- Approval, residual risk, and follow-up/review date:

## Procedure
1. Identify the dependency, current version, target version, and source.
2. Review changelog, advisories, compatibility, license, and transitive impact.
3. Record the current baseline.
4. Update in a controlled change with manifests and lockfiles reviewed.
5. Run relevant checks, tests, and regression.
6. Inspect the final diff for unrelated changes.
7. Record results, residual risk, and rollback approach.

## Guardrails
Do not blindly auto-merge major updates. Avoid arbitrary version changes without evidence. Review package integrity and source provenance.

## Dependencies
Sections 03, 07, 09–11, and 13.

## Acceptance evidence
A real dependency change has a documented reason, compatibility review, test evidence, and rollback path.

## Next action
Trial the workflow on a low-risk dependency in a non-production branch.
