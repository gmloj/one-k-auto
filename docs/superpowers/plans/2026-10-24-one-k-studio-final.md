# ONE K Studio — implementation plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox syntax.

**Goal:** Deliver a cinematic, mobile-first ONE K car-care landing page with a more polished showroom and service discovery.
**Architecture:** Keep the static HTML/CSS/Three.js page, current attributed 3D asset, latest mobile service dock, and GitHub Pages route. Add presentation styling and a client-side filter over existing service cards.
**Tech Stack:** HTML, CSS, vanilla JavaScript, Three.js 0.164.1, GitHub Pages.
**Spec:** `docs/superpowers/specs/2026-10-24-one-k-studio-design.md`

## Global Constraints
- Preserve ONE K identity, Arabic RTL, six services, and WhatsApp number 053 000 4764.
- Keep all touch/keyboard controls and the new mobile dock.
- Filter counts remain all 6, exterior 4, interior 2.
- Preserve truthful source attribution for the model; no unsupported claims.
- Keep root and `dist` HTML identical.

## Review Focus
- Phone widths 360/390 px: no page-level horizontal overflow; service dock still scrolls.
- Filter actions: only matching cards remain and selected state is announced.
- Reduced motion: existing reduced-motion behavior still works.
- Selecting and returning from services: current Three.js focus behavior remains intact.
- Model loading/failure: fallback and text controls remain available.

---

### Task 1: Cinematic presentation and copy
**Files:** Modify `index.html`, `dist/index.html`
- [ ] Add a subtle page-progress line, sculpted studio lighting, improved hero hierarchy, and premium service-card depth.
- [ ] Keep the newest mobile ordering, dock, scene status, and booking CTA.

### Task 2: Service filters
**Files:** Modify `index.html`, `dist/index.html`
- [ ] Add accessible All/Exterior/Interior controls.
- [ ] Categorize the six existing service cards and filter them without changing copy or destinations.

### Task 3: Verify and publish
- [ ] Parse inline scripts, confirm root/dist match, and check six services and WhatsApp targets.
- [ ] Inspect desktop and 390px/mobile rendering, filter behavior, and 3D fallback.
- [ ] Merge to main and verify the published GitHub Pages page.
