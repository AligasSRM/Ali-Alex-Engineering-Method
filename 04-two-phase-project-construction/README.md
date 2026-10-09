# Section 04 — Two-Phase Project Construction

**Status:** 🔴 RED — structure only; substantive work pending.

## Purpose
Separate full project structure planning from implementation and verification, including an explicit blueprint for the intended user-facing page experience before coding.

## Documents present
- PHASE-1-STRUCTURE.md — project map, modules, dependencies, risks, page-design gate, and acceptance evidence.
- PAGE-EXPERIENCE-AND-VISUAL-STRUCTURE.md — canonical template for page purpose, visual hierarchy, content/copy, components, routes, repository paths/assets, states, responsive behavior, accessibility, and design approval.
- PHASE-2-IMPLEMENTATION.md — bounded implementation increments, tests, review, and reporting.
- PHASE-TRANSITION-GATE.md — evidence-based gates from structure to implementation and from increment to acceptance.
- ACCEPTANCE-CRITERIA.md — evidence required to complete this section.
- STATUS.md — current state and next action.

## Dependencies
Sections 01–03 establish purpose, planning, and standards. Sections 05–07, 09–13, and 17 provide approval, problem-solving, verification, security, dependency, and release controls. Section 15 supports artifact traceability.

## Evidence and traceability
Use Section 02's canonical requirement traceability matrix for requirement IDs and verification evidence. Each structural module and implementation increment should reference stable requirement/decision/dependency IDs rather than copying competing status records. Record the exact repository, branch, baseline commit, environment, reviewer, and evidence location for each gate decision.

A gate decision must distinguish **PASS**, **FAIL**, **BLOCKED**, and **NOT APPLICABLE**. A NOT APPLICABLE decision requires rationale and authorized review; missing evidence is not a pass.

## Guardrail
A complete skeleton or approved visual blueprint is not a completed product; implementation, visual comparison, accessibility review, and functional testing remain separate.
