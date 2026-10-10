# Changelog and History

**Status:** RED — history policy drafted; repository conventions need validation.

## Entry schema
| Change ID | Date / version | Category | Summary / user impact | Requirement / decision IDs | Commit / PR | Test evidence | Release/deployment state | Owner / follow-up |
|---|---|---|---|---|---|---|---|---|
| CHG-001 | TBD | TBD | TBD | TBD | TBD | TBD | DRAFT / NOT RELEASED | TBD |

## Requirements
- Record user-visible or operationally material changes.
- Link changes to commits, decisions, issues, tests, and release notes where available.
- Distinguish added, changed, fixed, removed, security-related, and migration-impacting changes.
- Document breaking changes and required operator/user actions.
- Preserve an auditable history; do not rewrite records to conceal failed attempts or prior decisions.
- Keep sensitive implementation details and secrets out of public changelogs.
- Use the repository's established versioning/release convention where one exists.

## Corrections
Use explicit states such as DRAFTED, SAVED, COMMITTED, TESTED, DEPLOYED, RELEASED, REVERTED, or SUPERSEDED as applicable. Do not infer a later state from an earlier one; link to the authoritative commit, test run, or deployment record.

## Corrections
Correct inaccurate history transparently with a dated amendment or superseding entry. Avoid implying that a change was deployed merely because it was committed.

## Dependencies
Sections 05, 09–10, 12–14, and 17.

## Acceptance evidence
A reviewer can trace a material change from rationale through implementation, validation, and release status.

## Next action
Align the changelog convention with the repository's actual release model.
