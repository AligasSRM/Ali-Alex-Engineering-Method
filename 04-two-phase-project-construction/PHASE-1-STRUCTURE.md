# Phase 1 — Structural Blueprint

**Status:** 🔴 RED — process template only; no project structure is approved here.

## Purpose
Define the complete project map before implementing detailed functionality, so dependencies, boundaries, missing work, and the intended user-facing experience are visible.

## Required outputs
- Project purpose, users, and explicit scope boundaries.
- System/component map and responsibility boundaries.
- Section/module inventory with planned files and interfaces.
- Dependency graph and critical-path constraints.
- **Page experience and visual structure blueprint for every in-scope user-facing page/screen**, including layout hierarchy, content inventory, navigation, interactive controls, page states, responsive behavior, relevant design references, and approval.
- Verified repository/branch/entry points, planned file changes, routes, and asset sources; unknowns remain explicitly TBD.
- Cross-cutting requirements: security, privacy, accessibility, reliability, observability, and operations as applicable.
- Public launch readiness plan when applicable: canonical domain/HTTPS/DNS, Google search discoverability (metadata, robots.txt, sitemap.xml, Search Console), official domain email, mail authentication (SPF/DKIM/DMARC), contact-form routing, owners, and verification evidence.
- Support experience plan when applicable: support address/channel, contact form or ticket flow, ownership/response expectations, escalation, and an explicit decision on whether AI-assisted support is in scope; if AI is considered, map its data/tool permissions and human handoff before implementation.
- Acceptance criteria and verification approach for every module and user-facing journey.
- Risk, assumption, and decision registers.
- A traceable list of structural gaps and blockers.

## Page design gate
Before implementation of a user-facing page:
1. Inspect the actual repository, current route, components, styles, assets, and existing design system; record the branch/commit inspected.
2. Define the page purpose and map its regions from top to bottom, including navigation, content hierarchy, primary/secondary actions, footer or app shell, and responsive rearrangement.
3. Record exact or draft copy for headings, labels, buttons, help text, notices, and applicable loading/empty/success/error states. Mark unapproved copy OPEN.
4. Map every interactive element to a behavior, route/data dependency, feedback state, and verification method.
5. Link an approved wireframe, annotated screenshot, Figma file, or equivalent when visual precision matters; otherwise state that the blueprint is text-only and list unresolved design decisions.
6. Review accessibility, privacy, failure states, and acceptance evidence before the page enters implementation.

The canonical template is `PAGE-EXPERIENCE-AND-VISUAL-STRUCTURE.md`. This gate is part of Phase 1, not a new numbered methodology section.

## Public launch readiness gate
Before releasing an applicable public website:
1. Verify the actual domain, DNS, HTTPS, canonical host, and production/staging distinction.
2. Verify important public pages, metadata, robots.txt, sitemap.xml, and internal discoverability.
3. Verify Google Search Console ownership and record sitemap/URL inspection outcomes without claiming guaranteed indexing or ranking.
4. Decide required official email addresses and document provider ownership, recovery, and routing.
5. Verify required email DNS authentication and test real inbound/outbound messages and contact-form notifications.
6. Record owners, evidence, unresolved issues, and post-launch checks in `17-final-review-and-release/WEB-DISCOVERABILITY-AND-DOMAIN-EMAIL-READINESS.md`.

These gates belong to existing Sections 04 and 17, not a new numbered section.

## Structure inventory
| Area / module | Responsibility | Planned artifacts | Dependencies | Acceptance evidence | Status |
|---|---|---|---|---|---|
| TBD | TBD | TBD | TBD | TBD | Not started |

## Guardrails
- Phase 1 creates a reviewed blueprint, not a claim that the product works.
- Do not invent modules, scope, interfaces, copy, repository paths, assets, or external integrations without discovery evidence or owner approval.
- Identify which elements are confirmed, proposed, or unresolved.
- A text description is not equivalent to a visual design artifact when the layout requires precise review.
- Do not begin detailed page implementation while the page's purpose, structure, primary actions, and critical states remain unresolved.

## Acceptance criteria
- [ ] Every in-scope area is inventoried or explicitly excluded.
- [ ] Dependencies and ownership are mapped.
- [ ] Cross-cutting risks and acceptance gates are represented.
- [ ] Unresolved decisions and assumptions are visible.
- [ ] Each in-scope user-facing page has a page experience/visual structure blueprint, or an approved rationale for not needing one.
- [ ] Page layout, content, controls, routes, states, responsive behavior, and relevant accessibility needs are documented.
- [ ] Existing repository paths and assets are verified; unknowns are not guessed.
- [ ] Required design/reference artifacts are linked, or text-only limitations and open decisions are recorded.
- [ ] Public discoverability and domain email are planned with verification evidence or explicitly marked not applicable with rationale.
- [ ] Support channels and human escalation are planned, and AI support is explicitly approved, deferred, or marked not applicable with rationale.
- [ ] Project owner reviews the blueprint before Phase 2 begins.
