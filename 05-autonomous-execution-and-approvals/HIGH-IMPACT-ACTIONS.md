# High-Impact Actions

**Status:** 🔴 RED — catalogue drafted; operational controls and project-specific thresholds unverified.

## Purpose
Identify actions that must not be treated as routine execution because they can cause material, costly, external, security, privacy, or irreversible effects.

## High-impact categories
- **Destructive:** delete files, repositories, branches, data, backups, accounts, or resources; overwrite valuable state; perform migrations without a verified recovery path.
- **Financial:** incur charges, start paid trials that can convert to paid plans, purchase services, commit funds, or change billing.
- **External communication:** send email/messages, contact customers or acquisition targets, publish content, invite users, or make commitments on the user's behalf.
- **Security and access:** expose or rotate secrets, grant/revoke permissions, change authentication, alter security settings, or transfer ownership.
- **Production and live data:** activate production, deploy risky changes, process real transactions, modify live customer data, or disable safety controls.
- **Privacy and legal:** disclose personal/confidential information, change data retention, accept binding terms, or take actions with legal/regulatory implications.
- **Scope and architecture:** replace core technology, change the product's intended users or business model, or introduce a material dependency outside the approved plan.

## Required pre-action checklist
1. State the exact proposed action and target.
2. Explain expected outcome, likely impact, uncertainty, and alternatives.
3. Confirm backup/rollback or explain why none exists.
4. Identify environment and blast radius.
5. Obtain explicit approval before execution.
6. Execute only the approved action, then verify the result and report evidence.

## Durable execution record
For every approved high-impact action, preserve the approval ID/evidence, exact approved target and scope, operator, environment, start/end time, before/after state, backup/rollback evidence, commands or external action receipt where appropriate, verification outcome, residual risk, and follow-up owner. Redact secrets and unnecessary personal data from the record.

If the requested target, scope, recipient, cost, environment, or risk changes after approval, stop and re-confirm. A successful technical result does not retrospectively authorize an unapproved action.

## Emergency handling
A potential incident does not grant blanket permission for unrelated high-impact changes. Take only safe, already-authorized containment steps; otherwise preserve evidence, limit further exposure where clearly permitted, and escalate immediately.

## Dependencies
Coordinates with Section 03 engineering/security standards, Section 05 approval matrix, Section 11 privacy/secrets, Section 14 maintenance, and Section 17 final review/release.

## Acceptance evidence
A scenario-based review proves each listed category is recognized and gated, including paid-trial conversion, public publishing, production activation, and destructive operations.

## Next action
Compare this catalogue with the approval matrix and ensure each action maps to an explicit rule and evidence requirement.
