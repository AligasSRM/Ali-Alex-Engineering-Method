# Fail-Closed Rules

**Status:** 🔴 RED — rules drafted; system-specific failure paths need tests.

## Purpose
Ensure that when a required security, safety, identity, or authorization control fails, the system does not silently proceed as if the control passed.

## Default rules
- If authentication cannot be verified, reject the protected operation.
- If authorization is missing, stale, or ambiguous, deny access.
- If a mandatory safety/moderation/age check is unavailable or inconclusive, apply the explicitly defined safe fallback; do not bypass the requirement.
- If signature, integrity, or provenance validation fails, reject the affected input or action.
- If required audit evidence cannot be recorded, pause high-impact operations unless a documented, approved policy defines a safe alternative.
- If configuration is incomplete, disable the affected capability rather than pretending it is ready.
- If a dependency is degraded, restrict only the affected capability where safe; do not silently weaken security boundaries.
- Make denial and recovery paths observable without exposing secrets or sensitive data.

## Failure-mode matrix
| Control ID | Required precondition / signal | Failure or unknown condition | Denied/limited behavior | User/operator feedback | Audit evidence / alert | Recovery owner / re-entry condition | Test ID |
|---|---|---|---|---|---|---|---|
| CTRL-001 | TBD | TBD | TBD | TBD | TBD | TBD | TBD |

## Exception control
Any exception must be explicit, narrowly scoped, time-bounded where possible, approved by the proper authority, logged, and accompanied by compensating controls. Record the control/threat ID, residual risk, affected environments, expiry/review date, rollback/re-entry condition, and test evidence. No implicit fail-open behavior; exceptions cannot bypass applicable law or mandatory authorization.

## Dependencies
Sections 03, 05, 09–10, and all production/release sections.

## Acceptance evidence
Failure-injection scenarios demonstrate that missing or failed mandatory controls block the protected action and produce safe, auditable outcomes.

## Next action
Trace each mandatory control to a specific failure test and recovery owner.
