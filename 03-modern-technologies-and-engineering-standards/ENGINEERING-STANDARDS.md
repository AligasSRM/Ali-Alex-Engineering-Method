# Engineering Standards

**Status:** 🔴 RED — baseline template only; standards must be scoped to the project.

## Standards register
| Area | Standard / rule | Scope | Verification mechanism | Exception process |
|---|---|---|---|---|
| Code quality | TBD | TBD | Lint / review / static analysis as applicable | Documented approval |
| Formatting and consistency | TBD | TBD | Formatter or review | Documented approval |
| Types and contracts | TBD | TBD | Type checks / contract tests | Documented approval |
| Documentation | TBD | TBD | Review against changed behavior | Documented approval |
| Code review | TBD | TBD | Required review evidence | Documented approval |
| Observability and diagnostics | TBD | TBD | Logs / metrics / health checks as applicable | Documented approval |

## Classification and evidence requirements
Classify every entry as **mandatory**, **conditional**, or **recommended**. For conditional rules, record the triggering condition and how non-applicability is approved. For each selected standard, record its authoritative source URL, version/date, checked date, scope, accountable owner, enforcement point, evidence location, and review trigger. Do not label a recommendation as a hard gate without an approved decision.

## Exception / waiver record
- Rule ID and affected paths/components: TBD
- Business/technical rationale and alternatives considered: TBD
- Risk and compensating controls: TBD
- Approver and approval evidence: TBD
- Expiry or review date and closure condition: TBD

## Change principles
- Keep changes focused, reviewable, and traceable to requirements.
- Preserve existing behavior unless the change explicitly authorizes otherwise.
- Define tests before calling a change complete.
- Record rationale for exceptions; exceptions must not silently weaken security or data protection.

## Acceptance criteria
- [ ] Standards are specific, applicable, and verifiable.
- [ ] Tooling and review responsibilities are identified.
- [ ] Exception approval and expiration/review are documented.
- [ ] Standards are checked against the project's real stack and delivery process.
