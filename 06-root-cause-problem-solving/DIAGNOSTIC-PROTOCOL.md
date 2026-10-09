# Diagnostic Protocol

**Status:** 🔴 RED — draft procedure; field validation pending.

## Purpose
Move from symptoms to a supported causal explanation using explicit hypotheses and discriminating tests.

## Procedure
1. Establish the intake record and current baseline.
2. Reproduce the issue safely or document why it cannot be reproduced.
3. List competing hypotheses, each with supporting and contradicting evidence.
4. Rank hypotheses by evidence, impact, and test cost—not intuition alone.
5. Select the smallest safe test that distinguishes between hypotheses.
6. Record prediction, action, actual result, and interpretation.
7. Update the hypothesis list and avoid repeating equivalent tests.
8. Confirm the likely cause with evidence; if uncertain, report uncertainty rather than claiming certainty.
9. Propose a minimal fix, rollback strategy, and targeted regression plan.

## Safety and scope
Use Section 05 approval gates for high-impact actions. Never expose secrets in logs. Preserve a known-good state before risky modifications. Do not treat correlation as proof of causation.

## Required diagnostic log
| Diagnostic ID | Incident ID | Hypothesis / confidence before test | Supporting and contradicting evidence | Prediction / discriminating criterion | Safe test / environment | Actual result / evidence link | Conclusion / confidence after test | Next action / owner |
|---|---|---|---|---|---|---|---|---|
| DIAG-001 | TBD | TBD | TBD | TBD | TBD | TBD | TBD | TBD |

For each test, state what result would support, weaken, or falsify the hypothesis before running it. Record command/tool version and exit status where applicable. If the test cannot run, record the blocker; do not treat an unexecuted test as evidence.


## Dependencies
Sections 05, 09, 10, and 13; aligns with Section 07 patch review.

## Causal confidence
Use explicit labels such as **confirmed**, **strongly supported**, **provisional**, or **unknown**, with criteria defined by the project. Explain alternative causes not ruled out. A test passing after a change is evidence of behavior, but does not alone prove the proposed root cause.

## Acceptance evidence
A real issue has a traceable hypothesis-to-test record and a conclusion calibrated to the evidence.

## Next action
Compare with the three-attempt rule and research protocol to prevent duplicate or blind work.
