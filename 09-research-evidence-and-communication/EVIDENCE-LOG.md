# Evidence Log

**Status:** 🔴 RED — log schema drafted; evidence capture workflow untested.

## Purpose
Keep material claims traceable to the evidence that supports or contradicts them.

## Record schema
| Field | Required content |
|---|---|
| Evidence ID | Stable identifier |
| Claim | Exact claim being assessed |
| Source and provenance | File/path or URL, publisher/owner, command/tool, artifact ID, environment, and how it was obtained |
| Captured / checked time | Timestamp and time zone; relevant version/commit/environment |
| Evidence excerpt/result | Minimum relevant detail, with sensitive data redacted |
| Classification | Fact, inference, hypothesis, recommendation, or decision |
| Confidence / scope | High, medium, low, with rationale and the exact claim scope |
| Limitations | Missing context, freshness, scope, or possible bias |
| Status | Supports, contradicts, or does not resolve claim |
| Owner / review trigger | Accountable owner, next check, freshness/expiry trigger, or decision required |

## Rules
Assign a stable Evidence ID and link every material conclusion to the smallest relevant evidence set. Keep original source identity and capture time so a reviewer can distinguish source publication date from the date it was checked. If an artifact is unavailable, state that explicitly instead of reconstructing its contents from memory.

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
