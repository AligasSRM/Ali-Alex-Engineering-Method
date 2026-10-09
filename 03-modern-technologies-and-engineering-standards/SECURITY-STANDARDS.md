# Security Standards

**Status:** 🔴 RED — security policy template only; no compliance claim is made.

## Security baseline register
| Control area | Requirement / target | Scope | Verification evidence | Owner | Exceptions / remediation |
|---|---|---|---|---|---|
| Authentication and authorization | TBD from threat model | TBD | TBD | TBD | TBD |
| Secrets and credentials | Never commit secret values; use approved secret storage | All applicable environments | Repository scanning / configuration review | TBD | TBD |
| Input validation and output handling | TBD | TBD | Tests / review | TBD | TBD |
| Dependency and supply-chain risk | Inventory, review, and update dependencies | Applicable codebases | Audit / lockfile / CI evidence | TBD | TBD |
| Data protection and retention | Minimize access and retention; define handling by data class | TBD | Data-flow and access review | TBD | TBD |
| Logging and incident response | Avoid secret and unnecessary sensitive-data logging | TBD | Log/config review and incident plan | TBD | TBD |
| Backup, recovery, and failure behavior | Define based on criticality | TBD | Recovery test evidence | TBD | TBD |

## Standard selection
Choose applicable guidance based on product scope, threat model, jurisdiction, and deployment model. Cite authoritative versions and record the date checked. Do not state that the product is compliant or certified without a scoped assessment and evidence.

## Acceptance criteria
- [ ] Threats and data sensitivity are assessed for the project.
- [ ] Controls are mapped to verification methods.
- [ ] Secret handling and least-privilege access are documented.
- [ ] Exceptions have an owner, mitigation, and review date.
- [ ] Any compliance claim has defined scope and auditable evidence.
