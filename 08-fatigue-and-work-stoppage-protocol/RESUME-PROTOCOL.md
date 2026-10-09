# Resume Protocol

**Status:** 🔴 RED — draft procedure; handoff validation pending.

## Purpose
Resume paused work from verified current state rather than relying on memory or outdated notes.

## Procedure
1. Read the latest checkpoint and handoff notes.
2. Inspect the live repository, branch, status, relevant files, and current environment.
3. Compare observed state with the checkpoint; resolve differences before changing anything.
4. Confirm current scope, approvals, blockers, dependencies, and last known-good state.
5. Re-run only the minimum safe checks needed to establish the baseline.
6. Choose the next smallest authorized action and state its expected result.
7. Make the change, inspect the diff, and run relevant tests.
8. Update checkpoint, status, and evidence with the actual result.

## Guardrails
Do not assume prior plans were executed. Do not repeat already-passed work unless evidence suggests it is stale or a regression occurred. Re-confirm approval when material conditions have changed.

## Dependencies
Sections 02, 05–07, and 09–15.

## Acceptance evidence
A paused task is resumed with a confirmed baseline, no assumed completion, and an evidence-backed next action.

## Next action
Test the protocol with a real pause/resume cycle after the whole structure is built.
