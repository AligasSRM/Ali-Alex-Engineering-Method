# Acceptance Criteria — Section 17

**Status:** RED — criteria drafted; integrated release exercise pending.

- [ ] Readiness checklist covers scope, tests, dependencies, security/privacy, operations, recovery, and approvals.
- [ ] Final review records evidence, findings, dispositions, and authorized decision.
- [ ] GO/NO-GO/CONDITIONAL GO rules cannot bypass mandatory controls.
- [ ] Rollback or forward recovery is realistic and tested where feasible.
- [ ] Post-release verification is tied to the deployed artifact and observation window.
- [ ] Release record distinguishes approval, deployment, and verified outcome.
- [ ] Residual risks and deferred work are reconciled with Section 13.
- [ ] Locked sections and required approvals align with Sections 05 and 12.
- [ ] A representative release/recovery exercise is reviewed.

- [ ] Applicable public websites have evidence for canonical URL, DNS/HTTPS, indexable-page status, metadata, robots.txt, sitemap.xml, and important internal links.
- [ ] Google Search Console ownership and relevant sitemap/URL inspection outcomes are recorded; submission is not treated as a guarantee of indexing or ranking.
- [ ] Applicable domain email has tested inbound and outbound delivery, provider ownership/recovery, SPF, DKIM, DMARC, and contact/transactional notifications.
- [ ] Domain, search, and mail dependencies have named owners and recovery paths; no secrets are committed.
- [ ] Post-launch search and mail checks have an owner and review cadence.


## GREEN gate
A complete release lifecycle is traceable from readiness through final review, deployment, and post-release verification.

## LOCKED gate
Lock only after GREEN and successful review of the applicable release and recovery evidence.

## Dependencies
Sections 05–16 and 18.

## Next action
Run a controlled release simulation after the repository-wide structure review.
