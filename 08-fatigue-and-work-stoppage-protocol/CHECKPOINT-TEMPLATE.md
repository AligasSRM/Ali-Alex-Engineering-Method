# Checkpoint Template

**Status:** 🔴 RED — template drafted; resume reliability not yet tested.

Use this record whenever work pauses, changes hands, or reaches a meaningful milestone.

## Checkpoint
- **Checkpoint ID / parent checkpoint / handoff ID:**
- **Project/repository URL and branch:**
- **Date/time/time zone and environment:**
- **Current commit SHA / working-tree status / dirty paths:**
- **Runtime, tool versions, and relevant configuration source:**
- **Current phase and objective:**
- **Verified state:** only facts directly checked.
- **Last known-good commit/version or backup:**
- **Files/resources changed:**
- **Last verified command/test ID, exact command, exit status, and result:**
- **Evidence URLs/artifact locations and what each proves:**
- **Checks not run and why:**
- **Open blockers and evidence:**
- **Known risks and approval requirements:**
- **Decisions made and their source:**
- **Assumptions that remain unverified:**
- **Relevant dependencies/sections:**
- **Next smallest safe action (exact target, expected result, owner):**
- **Checkpoint freshness/revalidation triggers:**
- **Explicitly out of scope:**

## Rules
A checkpoint must state its limits and age. Revalidate it after branch/commit changes, environment/tool updates, deployment changes, a material approval/scope change, or a suspected regression. Do not assume a clean working tree or successful command unless it was observed and recorded.

## Rules
Never record a planned check as completed. Include no credentials or unnecessary personal data. Link to durable evidence where possible. If the checkpoint conflicts with the live repository, re-inspect the repository before resuming.

## Dependencies
Sections 05–06, 09, 12–15.

## Acceptance evidence
A new session or operator can resume by inspecting the stated evidence and confirming the live state without guessing.

## Next action
Validate by handing off a paused task and measuring whether the next action can be safely identified.
