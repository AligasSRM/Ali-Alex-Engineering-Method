# Versioning and Changelog

**Status:** RED — versioning policy drafted; baseline version not yet approved.

## Version record
- Lifecycle: PROPOSED / REVIEWED / APPROVED / EFFECTIVE / SUPERSEDED / WITHDRAWN.
For each method release, record:
- Version identifier, proposal ID, approval ID, and effective date/time zone (leave effective date unset until approved).
- Scope of changes, affected sections/files, linked requirement/decision IDs, and impact on dependency edges/approval precedence.
- Motivation and evidence.
- Compatibility or process changes for existing projects.
- Required approvals and review record.
- Validation results and known limitations.
- Migration/adoption instructions.
- Superseded version and rollback/restore approach.

## Change classification
- **Major:** incompatible governance or workflow change requiring explicit migration.
- **Minor:** additive capability or policy that preserves existing meaning.
- **Patch:** clarification or correction that does not change intended behavior.

These labels are a proposed convention until the baseline is approved.

## Rules
A version number assigned to a proposal does not make it effective. Record the exact source commit and approval evidence for every effective baseline. Use Section 15 for project-specific repository changes and release events; do not duplicate them here. If adoption is deferred, retain the current effective baseline and document the migration/revisit condition.

## Rules
Do not retroactively rewrite a prior approved version. Keep a canonical current version and an inspectable history. Record when a proposed change is not yet approved or effective.

## Dependencies
Sections 05, 12, 15–17, and this section's working agreement.

## Acceptance evidence
A sample release can be traced from approved proposal through validation, version assignment, and adoption instructions.

## Next action
Agree on a baseline version only after the initial method review and approval.
