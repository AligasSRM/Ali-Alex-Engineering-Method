# Customer Support and AI Assistance Readiness

**Status:** 🔴 RED — support-channel planning template only; no live support inbox, ticket flow, or AI assistant has been configured or tested.

## Purpose

Ensure users can contact the project owner/support team, receive and track help requests, and—only when approved—use an AI-assisted support experience with clear limitations and a safe escalation path.

A visible support address or AI chat widget is not proof that a message reaches a responsible person or that an issue is resolved.

## A. Support channels and ownership
- [ ] Decide which channels are required: domain email (for example, `support@yourdomain.com`), contact form, help center/FAQ, in-product support, or other approved channel.
- [ ] Name the accountable support owner and backup; define access permissions and mailbox/ticket ownership.
- [ ] Define supported topics, exclusions, languages, operating hours, expected response window, and urgent/security-reporting route.
- [ ] Test incoming messages from an external account, replies, attachments if accepted, spam filtering, bounces, and delivery to the responsible owner.
- [ ] Verify contact-form submissions end-to-end, including server-side validation, abuse/rate limiting, delivery failures, and a user-visible confirmation that does not falsely claim delivery.
- [ ] Define ticket/reference IDs, status tracking, duplicate handling, follow-up, closure, and reopening if a ticket system is used.
- [ ] Publish only approved contact details and response expectations; do not promise 24/7 coverage unless it is staffed and tested.

## B. AI-assisted support (only if approved for the product)
- [ ] Explicitly approve whether AI support is in scope; define the jobs it may and may not perform.
- [ ] Tell users clearly when they are interacting with AI; do not impersonate a human agent.
- [ ] Ground answers in approved, maintained help content and product documentation; identify uncertainty and avoid invented policy, account, billing, or status claims.
- [ ] Provide a clear route to human support or a support ticket, including when the AI is uncertain, fails repeatedly, or the user asks for a person.
- [ ] Define escalation triggers for security incidents, privacy requests, account access/recovery, billing disputes, safety concerns, legal requests, and other high-impact cases.
- [ ] Require authentication and authorization before exposing account-specific information or taking account actions; the AI must not bypass existing permissions or approvals.
- [ ] Do not let the AI claim it sent an email, opened a ticket, changed an account, issued a refund, or completed an action unless the connected system confirms success.
- [ ] Restrict tool/API access to the minimum necessary; require explicit authorization for consequential actions and keep auditable action records.
- [ ] Minimize personal data sent to AI providers; document provider, purpose, data flow, retention, training/use settings where available, and applicable contractual/jurisdictional review.
- [ ] Do not place passwords, authentication tokens, payment-card data, recovery codes, or unnecessary sensitive content in prompts, logs, analytics, or knowledge sources.
- [ ] Define retention/deletion, access control, abuse prevention, rate limits, prompt-injection defenses, and safe handling of user-supplied files/links.
- [ ] Test inaccurate answers, prompt injection, data leakage, unauthorized requests, unavailable providers, timeout/rate-limit errors, and escalation behavior before launch.
- [ ] Monitor answer quality, unresolved-contact rate, escalation success, failure rate, and user feedback without collecting unnecessary personal data.
- [ ] Assign a human owner to maintain support content and review high-impact or repeatedly failing cases.

## C. Evidence and release gate
| Check | Owner | Evidence / test record | Last checked | Status |
|---|---|---|---|---|
| Support address/inbox receives messages | TBD | TBD | TBD | OPEN |
| Replies and failure/bounce handling | TBD | TBD | TBD | OPEN |
| Contact form or ticket flow, if used | TBD | TBD | TBD | OPEN |
| Human escalation route | TBD | TBD | TBD | OPEN |
| AI scope/privacy/security approval, if used | TBD | TBD | TBD | OPEN |
| AI behavior and failure tests, if used | TBD | TBD | TBD | OPEN |
| Support ownership and response expectations | TBD | TBD | TBD | OPEN |

- [ ] Every enabled channel has an accountable owner and a real end-to-end test.
- [ ] AI support remains disabled until scope, privacy/security review, test evidence, and escalation are approved.
- [ ] Support and AI claims in the interface match what is actually operational.
- [ ] Post-launch ownership, monitoring, content maintenance, and incident escalation are recorded.

## Ownership boundaries
- Section 01 defines whether support and AI assistance are in product scope.
- Section 02 records approved, testable support requirements.
- Section 04 designs the contact/help experience and its UI states before implementation.
- Section 05 owns approval authority for consequential actions and exceptions.
- Section 09 owns evidence and truthful communication.
- Section 11 owns privacy, security, data handling, and access controls.
- Section 14 owns ongoing monitoring, support operations, incidents, and maintenance.
- Section 17 owns launch-readiness evidence and release decisions.

This checklist does not authorize an AI assistant, a ticketing service, or any specific provider. It does not claim that support channels currently work.

## Review record
- Product/domain: TBD
- Enabled support channels: TBD
- AI support approved: TBD
- Data/processors reviewed: TBD
- Owner/approver: TBD
- Date and evidence: TBD
- Decision: NOT REVIEWED

**Rule:** Keep RED until enabled channels have been tested against the actual deployment. AI support must not be represented as available before it is configured, reviewed, and verified.
