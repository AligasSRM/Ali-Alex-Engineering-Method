# Evidence Log

**Status:** 🔴 RED — log schema drafted; evidence capture workflow untested.

## Purpose
Keep material claims traceable to the evidence that supports or contradicts them.

## Record schema
| Field | Required content |
|---|---|
| Evidence ID | Stable identifier |
| Claim | Exact claim being assessed |
| Source | File, URL, command output, test artifact, or observed state |
| Date/version | When captured and relevant version |
| Evidence excerpt/result | Minimum relevant detail, with sensitive data redacted |
| Classification | Fact, inference, hypothesis, recommendation, or decision |
| Confidence | High, medium, low, with rationale |
| Limitations | Missing context, freshness, scope, or possible bias |
| Status | Supports, contradicts, or does not resolve claim |
| Follow-up | Next check or responsible decision |

## Rules
- Preserve enough context to reproduce the observation.
- Distinguish source evidence from an interpretation of it.
- A passing check supports only the behavior it actually tested.
- Record failed and contradictory evidence, not only successes.
- Do not store credentials, tokens, or unnecessary personal information.

## Dependencies
Sections 05–06, 10–12, and 17.

## Acceptance evidence
A reviewer can trace each material conclusion to a source and understand its limits.

## Next action
Use the log in a representative report and verify traceability.
