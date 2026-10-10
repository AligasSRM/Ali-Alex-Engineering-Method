# Current-State Audit

**Status:** 🔴 RED — audit template only; no project audit is claimed.

## Audit scope
Record the real state before modifying a project. Identify the target repository/project and audit boundary; record the branch and commit SHA, working-tree state, audit timestamp/time zone, operator, and commands/tools used. If a field cannot be verified, mark it `NOT CHECKED`, `UNAVAILABLE`, or `NOT APPLICABLE` with rationale—never infer a value.

| Area | Observed state / evidence | Risk or gap | Follow-up / owner |
|---|---|---|---|
| Repository and default branch | TBD | TBD | TBD |
| Working tree and recent commits | TBD | TBD | TBD |
| Runtime and toolchain versions | TBD | TBD | TBD |
| Dependencies and lockfiles | TBD | TBD | TBD |
| Configuration and environment | TBD; never paste secrets | TBD | TBD |
| Tests, build, lint, type checks | TBD | TBD | TBD |
| CI and recent workflow results | TBD | TBD | TBD |
| Deployment and live health | TBD / not applicable | TBD | TBD |
| Integrations and external services | TBD | TBD | TBD |
| Known issues and locked areas | TBD | TBD | TBD |

## Evidence rules
- Capture exact commands, outputs, links, timestamps, and commit identifiers when relevant.
- Distinguish not checked, unavailable, failed, and passed.
- Do not expose credentials, tokens, private user data, or secret values.
- Never infer that a deployment works from a successful local build alone.

## Acceptance criteria
- [ ] Audit scope and timestamp are recorded.
- [ ] Every applicable row has evidence or is explicitly marked not checked/not applicable.
- [ ] Existing failures and locked sections are identified before edits.
- [ ] Baseline test/build results are captured where possible.
- [ ] Repository, branch, commit, and working-tree state are recorded before edits.
- [ ] Evidence distinguishes local, CI, staging, and live-production observations.
- [ ] Audit artifacts contain no secrets or unnecessary personal data.
- [ ] Any audit gap that could invalidate implementation is recorded as a blocker in Section 13.
- [ ] Reviewer confirms the audit is sufficient for planning.

## Next action
Run the audit against the actual target project before any implementation.
