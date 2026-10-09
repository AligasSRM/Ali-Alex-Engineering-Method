# Documentation Standards

**Status:** RED — standards drafted; repository-wide audit pending.

## Purpose
Make documentation accurate, navigable, maintainable, and useful for implementation and operations.

## Requirements
- Give material artifacts a stable ID, owner, lifecycle state, last-reviewed date, and canonical source location where appropriate.
- State purpose, scope, audience, prerequisites, and owner where relevant.
- Distinguish verified facts, assumptions, decisions, examples, and open questions.
- Keep instructions reproducible and identify the version/environment, repository/commit, and prerequisites they apply to.
- Link to authoritative sources and internal dependencies; record source checked date for time-sensitive claims.
- Avoid duplicated canonical content; link to the source of truth.
- Mark obsolete guidance clearly and define its replacement.
- Never include live credentials or unnecessary personal data.
- Keep status and acceptance claims aligned with evidence.

## Review triggers
For material changes, review affected docs in the same change where practical and link the requirement/decision, changed behavior, test evidence, and release disposition. Mark stale guidance with a replacement link and removal/review date rather than silently deleting decision history.

## Review triggers
Review when behavior, architecture, ownership, provider APIs, security controls, or acceptance criteria change.

## Dependencies
Sections 01–03, 09–14, and 18.

## Acceptance evidence
A documentation sample is reviewed for accuracy, traceability, clarity, and consistency with implementation.

## Next action
Apply the standard to a real section and record findings.
