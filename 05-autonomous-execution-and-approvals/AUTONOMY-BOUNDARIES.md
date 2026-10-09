# Autonomy Boundaries

**Status:** 🔴 RED — structure drafted; policy not yet validated against real projects.

## Purpose
Define what the assistant or project operator may execute independently after the user has approved the project scope.

## Working policy
- **Proceed within scope:** inspect accessible project state, map files and dependencies, draft plans, make reversible changes explicitly included in the approved task, and run non-destructive checks.
- **Pause and ask:** when scope or architecture would materially change; a task creates a cost or subscription; a message or other action contacts an external party; a destructive or irreversible operation is proposed; security permissions or production activation change; secrets or sensitive data may be exposed; or user intent and consequences are unclear.
- **Never infer consent** from silence, urgency, previous approval of a different action, or technical ability to perform an action.
- Prefer the smallest reversible action that satisfies the approved objective. Keep unrelated files and systems untouched.
- If a blocker prevents safe execution, stop that action, preserve evidence, and report options rather than bypassing the control.

## Required execution record
For each meaningful task, record the approved scope, intended action, risk/reversibility, checks performed, observed result, and any approval still needed.

## Dependencies
Sections 01–02 define purpose, scope, requirements, risks, and the current-state audit. Coordinate with Sections 11–13 for security, status gates, dependencies, and blockers.

## Acceptance evidence
A real-project walkthrough demonstrates that in-scope reversible work proceeds while each approval-required case is paused. Until then, this document is a draft and the section remains RED.

## Next action
Cross-check these boundaries against the approval matrix and high-impact action catalogue, then validate them on a real project without performing unapproved high-impact actions.
