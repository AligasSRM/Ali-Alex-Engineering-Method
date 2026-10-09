# Threat Model

**Status:** 🔴 RED — framework drafted; project-specific threat analysis pending.

## Purpose
Identify assets, actors, trust boundaries, likely threats, and controls before implementation or release.

## Required model
- **Assets:** credentials, personal/confidential data, source code, infrastructure, transactions, and service availability.
- **Actors:** legitimate users, operators, service identities, external providers, attackers, and accidental insiders.
- **Trust boundaries:** browser/client, API, worker/service, database/storage, third-party integrations, admin surfaces, and deployment pipeline.
- **Entry points:** public endpoints, uploads, callbacks/webhooks, authentication flows, administrative actions, dependency/build systems.
- **Threat scenarios:** unauthorized access, privilege escalation, data leakage, tampering, replay, denial of service, supply-chain compromise, and unsafe failure behavior.
- **Controls:** prevention, detection, containment, recovery, and evidence.
- **Residual risk:** likelihood, impact, uncertainty, owner, and acceptance authority.

## Threat register
| Threat ID | Asset / data-flow ID | Actor / entry point / trust boundary | Abuse scenario / impact | Likelihood / confidence | Existing control / gap | Test ID / evidence | Owner / residual risk / disposition |
|---|---|---|---|---|---|---|---|
| THR-001 | TBD | TBD | TBD | TBD | TBD | TBD | TBD |

## Method
Model data flows and attacker goals; prioritize realistic paths and material impact. Do not treat a checklist as proof that threats are eliminated. Review the model when architecture, data, permissions, dependencies, or external integrations change.

## Dependencies
Sections 02–05, 09–10, and 14–17.

## Change triggers
Re-review after changes to architecture, identity/permission boundaries, data categories/flows, external providers, dependency/build pipeline, public endpoints, or a material incident. Record model version, reviewer, date, and what changed.

## Acceptance evidence
A real project has a reviewed data-flow/threat model, mapped controls, test coverage, and explicit residual risks.

## Next action
Apply the model to the actual architecture before any production activation.
