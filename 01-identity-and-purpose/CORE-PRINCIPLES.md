# Core Principles

**Status:** 🔴 RED — initial checklist only.

Principles to evaluate and approve:
- User goals before feature count.
- Clear and consistent user experience.
- Integration by design, not by accidental coupling.
- Security and privacy by default.
- Accessibility and responsive behavior.
- Evidence-based decisions and honest status reporting.
- Maintainability and controlled complexity.
- Measurable reliability and graceful failure.
- Transparent costs, limits, and permissions where applicable.
- Continuous improvement without unnecessary rewrites.

## Operationalization matrix

| Candidate principle | Observable decision rule / question | Evidence needed | Owner / approval | State |
|---|---|---|---|---|
| User goals before feature count | Does this capability solve a validated user need and have a measurable outcome? | Requirement/source and acceptance method | TBD | Draft |
| Security and privacy by default | What data, permissions, threats, and retention are necessary, and what is the least-privilege design? | Section 11 threat/privacy review | TBD | Draft |
| Accessibility and responsive behavior | Which supported input methods, assistive technologies, and viewport states must pass? | Section 03 standards and Section 10 test evidence | TBD | Draft |
| Evidence-based decisions | Which source or test supports the claim, and what remains uncertain? | Evidence record in Section 09 | TBD | Draft |
| Maintainability and controlled complexity | Who owns the change, what dependencies are added, and how is it rolled back? | Design/change record and regression evidence | TBD | Draft |
| Measurable reliability and graceful failure | What happens on timeout, invalid input, dependency outage, and partial failure? | Failure-mode tests and recovery evidence | TBD | Draft |

These are candidates, not approved product requirements. Approve, amend, or reject each applicable rule with a recorded rationale; do not treat the examples as product-specific decisions.
