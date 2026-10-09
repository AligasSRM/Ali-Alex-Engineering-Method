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
