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
- [ ] Project owner reviews the blueprint before Phase 2 begins.
