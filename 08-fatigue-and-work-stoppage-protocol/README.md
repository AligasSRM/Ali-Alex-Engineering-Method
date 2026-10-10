# Section 08 — Fatigue and Work-Stoppage Protocol

**Status:** 🔴 RED — structure only; substantive work pending.

## Purpose
Stop unproductive loops safely and preserve enough context to resume without guesswork.

## Planned documents
- STOP-WORK-TRIGGERS.md — repeated failures, fatigue, and loss of progress.
- CHECKPOINT-TEMPLATE.md — known-good state and current evidence.
- RESUME-PROTOCOL.md — fresh inspection and next safe step.
- HANDOFF-NOTES.md — concise record of status and blockers.
- ACCEPTANCE-CRITERIA.md — evidence required to complete this section.
- STATUS.md — current state and next action.

## Dependencies
Applies across all sections and projects.
## Continuity integrity
A checkpoint is a snapshot, not proof that the live system still matches it. Record repository/branch/commit, working-tree state, environment and tool versions, timestamp/time zone, last verified command/result, evidence links, owner, and one next safe action. At resume, inspect live state and invalidate stale assumptions before editing.

## Guardrail
At a stop point, record verified state, not assumptions or unverified plans. Approval does not transfer automatically between targets, environments, operators, or changed conditions.
