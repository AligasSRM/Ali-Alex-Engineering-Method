# Web Discoverability and Domain Email Readiness

**Status:** 🔴 RED — release-planning template only; no live domain, search indexing, or email service has been verified.

## Purpose

Make a website findable through search engines and ensure its official domain email is planned and operational where the project needs these capabilities. A published URL alone does not prove search indexing, and an address written on a page does not prove mail delivery.

Use this checklist for public websites and products that need public discoverability or domain-based email. Record a reasoned not-applicable decision when either capability is intentionally out of scope.

## A. Website identity and domain
- Canonical production URL and preferred hostname (www/non-www) are recorded.
- Domain ownership, DNS control, hosting target, TLS/HTTPS, redirects, and renewal owner are verified.
- The canonical URL is consistent across redirects, page metadata, sitemap, and public contact details.
- Production and preview/staging environments are distinguished; staging/private pages must not be accidentally indexed.

## B. Search engine discoverability
- [ ] Site can be reached over HTTPS without authentication or unexpected blocking.
- [ ] Important public pages return the intended HTTP status; unavailable routes do not silently return false success.
- [ ] Each indexable page has an accurate title, useful meta description, clear heading hierarchy, and appropriate canonical URL.
- [ ] `robots.txt` is checked for accidental blocking and does not serve as a security boundary.
- [ ] `sitemap.xml` contains canonical, indexable URLs only and is updated with the site.
- [ ] Internal links make important pages discoverable; broken links and redirect chains are checked.
- [ ] Pages have useful, non-duplicated content; metadata does not promise unsupported features.
- [ ] Images have suitable alternative text where meaningful; structured data is used only when accurate and applicable.
- [ ] Mobile layout, loading performance, accessibility, and user-visible errors are reviewed.
- [ ] Google Search Console ownership is verified using an approved method and least-privilege access.
- [ ] Sitemap is submitted in Search Console where appropriate; important URLs are inspected and indexing issues reviewed.
- [ ] Search Console verification method, property, sitemap submission, date, and outstanding errors are recorded without storing secrets.
- [ ] Indexing is monitored after launch; indexing is requested where appropriate but never treated as guaranteed.
- [ ] Analytics/cookie consent and privacy disclosures are handled according to applicable requirements if analytics are deployed.

## C. Domain email and deliverability
- [ ] Required addresses and roles are decided (for example, `info@`, `support@`, `privacy@`, `billing@`); only needed mailboxes/aliases are created.
- [ ] Email provider, account owner, billing/renewal, recovery route, MFA, and access permissions are documented.
- [ ] Domain DNS records required by the chosen provider are installed and verified.
- [ ] SPF authorizes the intended sending services and avoids multiple conflicting SPF records.
- [ ] DKIM signing is enabled for each relevant sending service and verified.
- [ ] DMARC is published with an intentional policy and reporting destination; start cautiously where necessary, then strengthen after legitimate senders are inventoried and alignment is verified.
- [ ] SPF/DKIM/DMARC alignment and message authentication are tested using real provider-supported checks.
- [ ] Inbound mail is tested from an external account; outbound mail is tested to independent providers, including spam-folder and bounce handling.
- [ ] Replies, contact-form notifications, password resets, transactional messages, and support routing are tested where applicable.
- [ ] From/reply-to addresses, signatures, footer contact details, and public privacy/contact pages are consistent.
- [ ] Account recovery, MFA, unauthorized access response, mailbox retention, and sensitive-data handling are defined.
- [ ] Email delivery logs and bounce/complaint signals are available to the authorized operator; credentials and private message content are not added to public repositories.

## D. Contact and trust
- Public contact details are intentional, current, and approved for publication.
- Contact forms explain what information is collected, where it goes, and expected response handling.
- A form's successful UI message is not treated as proof of delivery; notification receipt is verified end-to-end.
- Privacy, terms, support, and legal pages are included when applicable to the actual product and jurisdiction.
- Public claims, business identity, and trust marks are accurate; no fabricated address, certification, or endorsement is used.

## E. Ownership, evidence, and launch gate
| Check ID | Capability | Owner | Verified target / property | Evidence / test ID | Last checked (timestamp/time zone) | Outcome / status |
|---|---|---|---|---|---|
| WEB-001 | Domain/DNS/HTTPS | TBD | TBD | TBD | TBD | NOT CHECKED |
| WEB-002 | Google Search Console | TBD | TBD | TBD | TBD | NOT CHECKED |
| WEB-003 | Sitemap/robots/canonical | TBD | TBD | TBD | TBD | NOT CHECKED |
| MAIL-001 | Domain email/inbound/outbound | TBD | TBD | TBD | TBD | NOT CHECKED |
| MAIL-002 | SPF/DKIM/DMARC | TBD | TBD | TBD | TBD | NOT CHECKED |
| WEB-004 | Contact forms/notifications | TBD | TBD | TBD | TBD | NOT CHECKED |

- [ ] Every applicable capability has an owner, verification method, and evidence.
- [ ] Required checks pass before launch or have an explicitly approved, low-risk exception.
- [ ] Known indexing delays, search engine discretion, and residual email deliverability risks are documented.
- [ ] Post-launch checks are scheduled and tied to the deployed domain and release.
- [ ] Secrets, DNS tokens, verification tokens, private mailbox contents, and recovery codes are never committed to the repository.

## Boundaries and dependencies

- Section 01 defines purpose, audience, and whether public discovery/contact are in scope.
- Section 02 records requirements and verification methods.
- Section 03 defines relevant technology, accessibility, privacy, and operational standards.
- Section 04 plans the actual page experience, routes, assets, and implementation.
- Section 05 defines approval authority and exceptions.
- Section 11 owns security and privacy controls.
- Section 13 tracks domain, DNS, mail, hosting, and search-provider dependencies/blockers.
- Section 14 owns ongoing maintenance, observability, and incident operations.
- Section 17 owns release readiness, evidence, and post-release verification.

This document owns the launch-readiness checklist and evidence for public discoverability/domain email. It does not replace page design, product requirements, security policy, or actual provider setup.

## Review record
- Review ID / target release / environment:
- DNS/mail provider documentation checked date:
- Test IDs and evidence artifact links:

- Product/domain: TBD
- Canonical URL: TBD
- Email provider and required addresses: TBD
- Search property: TBD
- Reviewer / approver: TBD
- Date: TBD
- Decision: NOT REVIEWED

**Rule:** Keep this document RED until it has been applied to the actual domain and email setup with inspectable evidence. This template does not claim that the site is indexed or that email is configured.
