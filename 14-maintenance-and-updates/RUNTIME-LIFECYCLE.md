# Runtime Lifecycle

**Status:** RED — lifecycle guidance drafted; actual runtime inventory pending.

## Inventory
| Component ID | Runtime/framework/platform/tool and version | Official lifecycle URL / checked date | Support/EOL status and date | Consumers / compatibility evidence | Upgrade trigger / owner | Risk / next review |
|---|---|---|---|---|---|---|
| LIFE-001 | TBD | TBD | TBD | TBD | TBD | TBD |


For each runtime, framework, platform, database, and build tool, record version, support policy, published end-of-life date, upstream source, upgrade path, and dependent components.

## Policy
- Prefer actively supported versions compatible with product requirements.
- Verify lifecycle dates against official maintainer sources.
- Plan upgrades before support ends, allowing time for compatibility and regression checks.
- Assess security fixes, breaking changes, deployment constraints, and rollback options.
- Do not upgrade solely to chase the newest version without a need and compatibility review.
- Treat end-of-life runtimes as an explicit risk; define mitigation and a dated migration decision.

## Dependencies
Sections 03, 10, 11, and 13.

## Acceptance evidence
Critical runtimes have verified support status, owners, and a risk-based upgrade plan.

## Next action
Inventory deployed and development runtimes and verify lifecycle status from official sources.
