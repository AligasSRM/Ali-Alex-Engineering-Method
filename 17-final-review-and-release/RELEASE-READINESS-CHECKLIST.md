# Release Readiness Checklist

**Status:** RED — checklist drafted; release-specific validation pending.

## Scope and evidence
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

## Decision
Record **GO**, **NO-GO**, or **CONDITIONAL GO** with scope, evidence, decision authority, conditions, owner, and expiry/review point. Conditional approval must not bypass mandatory safety, legal, security, or approval controls.

## Dependencies
Sections 05, 09–16, and 18.

## Acceptance evidence
A release decision can be independently reconstructed from its checklist and evidence.

## Next action
Apply this checklist to a representative release in a safe environment.
