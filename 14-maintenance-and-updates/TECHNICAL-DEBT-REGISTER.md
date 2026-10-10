# Technical Debt Register

**Status:** RED — register template drafted; inventory pending.

## Required fields
- Lifecycle state: OPEN / INVESTIGATING / PLANNED / ACCEPTED RISK / IN PROGRESS / RESOLVED / REOPENED.
- Debt ID and affected component.
- Description and evidence.
- Root cause or historical context, if known.
- Impact and affected requirement/threat/dependency IDs: reliability, security, privacy, performance, maintainability, delivery, or cost.
- Likelihood, urgency, and affected workflows.
- Workaround and limitations.
- Remediation options and estimated effort/uncertainty.
- Dependencies, owner, priority, and review date.
- Risk-acceptance authority/approval ID and expiry/review date if accepted; reassessment trigger and closure evidence.

## Prioritization
Accepted-risk entries must identify an accountable risk owner, compensating controls, expiry/review trigger, and evidence needed to close. An expired risk acceptance is not automatically renewed.

## Prioritization
Prioritize by expected harm, likelihood, compounding cost, and strategic relevance—not age or visibility alone. Do not disguise mandatory risk remediation as optional debt. Reassess when the component changes or the workaround becomes unsafe.

## Dependencies
Sections 06–07, 09–11, and 13.

## Acceptance evidence
Material debt has an owner, evidence, priority rationale, and remediation or accepted-risk path.

## Next action
Inventory known debt from incidents, reviews, tests, and deferred work.
