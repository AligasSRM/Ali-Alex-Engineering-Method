# Release Readiness Checklist

**Status:** RED — checklist drafted; release-specific validation pending.

## Scope and evidence
- [ ] Release ID, candidate commit, artifact/build identity, environment, and observation window are fixed.
- [ ] Each checklist item has an outcome (PASS / FAIL / BLOCKED / NOT CHECKED / NOT APPLICABLE with rationale), evidence ID/link, owner, and last-checked time.
- [ ] Release scope, version/commit, and intended environment are explicit.
- [ ] Applicable acceptance criteria are met with inspectable evidence.
- [ ] Required tests ran; failed, skipped, and untested checks are visible.
- [ ] Dependencies, migrations, configuration, and provider availability are reviewed.
- [ ] Security, privacy, authorization, and safety gates pass.
- [ ] Monitoring, alerting, support ownership, and incident response are ready.
- [ ] Backup/recovery and rollback or forward-recovery procedures are verified.
- [ ] Cost exposure, external commitments, and user-impact risks are understood.
- [ ] Required approvals are recorded.
- [ ] Known limitations and residual risks have an authorized disposition.
- [ ] Release notes and operator/user instructions are prepared.
- [ ] No blocker contradicts the release decision.

## Public website and domain email (when applicable)

- [ ] Canonical production URL, DNS/HTTPS, and staging-versus-production indexing boundaries are verified.
- [ ] Important public pages, metadata, canonical URLs, robots.txt, sitemap.xml, and internal links are checked.
- [ ] Google Search Console ownership and sitemap/URL inspection outcomes are recorded; indexing/ranking are not guaranteed.
- [ ] Official domain email ownership and routing are documented; real inbound and outbound messages are tested.
- [ ] SPF, DKIM, and DMARC are configured and verified for the chosen provider.
- [ ] Contact-form notifications, replies, and bounce handling are tested where applicable.
- [ ] Public contact details and privacy notices are approved; owners and recovery paths are documented.
- [ ] No DNS/search verification tokens, mailbox credentials, or recovery codes are committed to the repository.

## Customer support and AI assistance (when applicable)

- [ ] Published support channels, accountable owner/backup, response expectations, and escalation route are approved.
- [ ] Support inbox and contact/ticket flows are tested end-to-end, including replies, delivery failures, and user-facing confirmation.
- [ ] If AI support is enabled, its scope, disclosure, approved knowledge sources, privacy/security review, permissions, and human escalation are approved and tested.
- [ ] AI support cannot claim external actions succeeded without confirmation from the connected system; high-impact requests follow authorization and human-review rules.
- [ ] AI failure, unsafe/inaccurate answers, privacy leakage, prompt injection, provider outage, and escalation scenarios are tested; an accountable human maintains support content.
- [ ] No support/AI capability is advertised as operational until its real deployment and evidence are verified.

## Decision
Record **GO**, **NO-GO**, or **CONDITIONAL GO** with release ID, exact commit/artifact/environment, evidence, decision authority, conditions, condition owners, expiry/review point, and rollback trigger. CONDITIONAL GO must identify why the condition is safe and cannot bypass a mandatory control. Any material candidate change invalidates affected evidence until rerun. Conditional approval must not bypass mandatory safety, legal, security, or approval controls.

## Dependencies
Sections 05, 09–16, and 18.

## Acceptance evidence
A release decision can be independently reconstructed from its checklist and evidence.

## Next action
Apply this checklist to a representative release in a safe environment.
