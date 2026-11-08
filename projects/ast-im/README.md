# AST-IM · redesign workspace

Purpose: design and implement a **new standalone visual prototype** of the existing AST-IM landing page, then separately migrate approved design to Flexbe. This folder is the canonical project handoff to Codex; do not confuse it with the demo concepts CONTOUR/FORMA/SILVA.

## Read in order
1. AGENTS.md (hard boundaries)
2. BUSINESS_FACTS.md (approved factual claims)
3. CONTENT_MASTER.md (approved structure and available copy)
4. DESIGN_BRIEF.md (art direction)
5. QUIZ_SPEC.md (existing functional contract)
6. ASSETS.md (photo/review provenance)
7. FLEXBE_STATE.md (current state)
8. ACCEPTANCE.md (quality gate)
9. Root DESIGN_SYSTEM.md, CONCEPTS.md, FLEXBE.md, preview.css, and concepts/engineering.html.

## Source reliability
- Project instruction: ChatGPT Library “Инструкция по работе с лендингом.md” v1.1 (2026-11-07), authoritative for business facts and constraints, but **stale on version IDs and contact branches**.
- Current Flexbe branch inspected 2026-11-08, editor version 12723607, published 12700593; authoritative for current page layout and content.
- Prior approved master document v1.0 has **not yet been retrieved as a standalone source**. CONTENT_MASTER.md is an interim reconstructed outline, not an authenticated verbatim master document.
- Design system: repo root Architectural Precision v4.1.

## Work stages
A. Inventory sources, preserve existing texts, build source-to-section traceability.
B. Develop high-quality complete HTML/CSS/JS prototype under projects/ast-im/prototype/ without modifying existing lab pages.
C. Run desktop/mobile visual QA and show preview. Do not call it verified if browser checks were not run.
D. After explicit approval, plan Flexbe migration; no direct publication.
