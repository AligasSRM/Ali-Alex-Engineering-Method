# Three-Attempt Rule

**Status:** 🔴 RED — rule drafted; operational examples and edge cases unvalidated.

## Purpose
Prevent unproductive repetition while ensuring investigation becomes more evidence-driven after failure.

## Rule
- **Attempt 1:** Test the best-supported initial hypothesis with a safe, focused diagnostic or fix.
- **Attempt 2:** If it fails, document why and try a materially different hypothesis or method.
- **After two failures:** Stop repeating local variations. Broaden research using official documentation, release notes, issue trackers, and reliable alternatives; re-check assumptions and environment.
- **Attempt 3:** Proceed only when the broader research produces a new, evidence-based approach. State what changed and what result would confirm or reject it.
- **If attempt 3 fails:** Stop the loop. Provide evidence, what was ruled out, unresolved uncertainty, risk, and realistic next options. Do not quietly start attempt 4.

## Exceptions
Immediate safety/security risks, destructive potential, or unclear authorization require stopping and escalating sooner. Read-only evidence gathering may continue when safe and useful, but it must not disguise a fourth implementation attempt.

## Required record
For each attempt: hypothesis, meaningful difference from prior attempts, evidence, action, result, and decision.

## Dependencies
Section 05 escalation; Section 07 patch discipline; Section 08 stop-work; Section 09 research/evidence.

## Acceptance evidence
Scenario tests confirm that equivalent retries are rejected, research follows two distinct failures, and a failed third attempt produces a stop report.

## Next action
Validate this rule against the escalation and work-stoppage protocols.
