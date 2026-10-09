# Claim Classification

**Status:** 🔴 RED — definitions drafted; usage consistency pending.

## Purpose
Prevent facts, interpretations, possibilities, and decisions from being presented as interchangeable.

## Classifications
- **Fact:** directly observed or established by a reliable source; state the evidence and scope.
- **Inference:** a reasoned conclusion from facts; show the reasoning and uncertainty.
- **Hypothesis:** a testable explanation not yet confirmed; state what would support or reject it.
- **Recommendation:** a proposed course of action based on stated objectives, evidence, trade-offs, and constraints.
- **Decision:** an authorized choice by the relevant decision-maker; record scope and limits.
- **Plan:** intended future work; never report it as completed.
- **Unknown:** a material point for which evidence is missing or inconclusive.

## Claim record fields
- Claim ID and exact wording:
- Classification and lifecycle: DRAFT / UNDER REVIEW / SUPPORTED / CONTRADICTED / UNRESOLVED / SUPERSEDED:
- Supporting and contradicting evidence IDs:
- Reasoning, confidence, scope, and assumptions:
- Owner/reviewer and last checked date:
- Revisit trigger or expiry for time-sensitive claims:

## Language controls
Use “verified” only when the check was actually performed and its result observed; identify the exact scope, environment, and time of that check. Use “likely” or “provisional” when causal confidence is limited. State “not checked” or “blocked” when applicable. Do not use GREEN, complete, deployed, connected, or live to imply evidence that does not exist.

## Dependencies
Sections 05–06, 10, 12–13, and 17.

## Acceptance evidence
Review a report and confirm every material claim is classified appropriately and backed by evidence or clearly labeled as uncertain.

## Next action
Cross-check terminology against status reporting and release gates.
