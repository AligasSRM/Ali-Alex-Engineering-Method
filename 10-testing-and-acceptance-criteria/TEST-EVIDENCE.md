# Test Evidence

**Status:** 🔴 RED — evidence template drafted; real execution record pending.

## Required record
- **Test run ID / CI job URL / artifact retention location:**
- **Exact commit SHA and working-tree/build artifact identity:**
- **Linked requirement, risk, test-case, defect, and change IDs:**
- Project, branch/commit, and change under test.
- Date/time/time zone, runtime/tool versions, OS/container/image, configuration source, and environment.
- Exact command or test action.
- Test level and requirements/risks covered.
- Expected result and observed result.
- Pass/fail/blocked/skipped/not-run status and reason.
- Exit code, relevant output, logs, and artifact links.
- Mocked dependencies, test fixtures, and limitations.
- Failures, flaky behavior, and follow-up actions.
- Reviewer/approval and release relevance where applicable.

## Evidence rules
If a test is rerun, preserve distinct run IDs and results; do not overwrite a failed run with a later pass without noting the sequence and cause. Identify flaky retries, test quarantine, changed fixtures, and manual overrides. Record evidence freshness and whether the exact tested commit is still the candidate commit.

## Evidence rules
Preserve useful output without leaking secrets or personal data. Never convert a skipped, blocked, or unexecuted test into a pass. A successful result applies only to the tested commit, environment, and scenario. If the commit changes after testing, rerun the checks affected by the change.

## Dependencies
Sections 09, 11–13, and 17.

## Acceptance evidence
A reviewer can reproduce the run and verify that the stated status matches the actual evidence.

## Next action
Attach this record to a real test run and verify traceability to requirements.
