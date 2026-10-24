# ONE K Studio Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (- [ ]) syntax.

**Goal:** Rebuild the ONE K landing page as a cinematic, mobile-first interactive car-care studio experience.

**Architecture:** Keep the current static HTML/CSS/Three.js page and GitHub Pages deployment. Add licensed generic unbranded car/studio assets, preserve accessible HTML service controls and WhatsApp booking, and keep root and `dist` pages byte-identical.

**Tech Stack:** HTML, CSS, vanilla JavaScript, Three.js 0.164.1, GLTF/GLB assets, GitHub Pages.

**Spec:** `docs/superpowers/specs/2026-10-24-one-k-studio-design.md`

## Global Constraints
- Arabic RTL content, current ONE K identity, and booking number 053 000 4764 remain.
- Use a generic coupe without a car-maker logo; verify reuse rights before committing any model.
- Do not invent business claims, prices, guarantees, testimonials, customers, or statistics.
- Keep all six service choices available with camera focus and a visible text alternative.
- Provide a lightweight fallback and respect prefers-reduced-motion.
- Update `index.html` and `dist/index.html` together.

## Review Focus
- Model or CDN unavailable: fallback still lets visitors choose and book every service.
- Narrow phone viewport: horizontal service strip works without page-level horizontal overflow.
- Reduced motion: camera and decorative animation stop or shorten.
- Keyboard activation: every hotspot and service selector remains reachable and has an accessible label.
- Repeated selections: switching services and returning reset camera, glass, and body visibility correctly.

---

### Task 1: Verify and prepare visual assets
**Files:**
- Modify: `assets/MODEL-LICENSE.md`
- Create: `assets/one-k-coupe.glb` (only if the verified source is usable)
- Create: `assets/studio.webp` and service imagery as needed

- [ ] Confirm model is unbranded and license permits commercial reuse; record author, source, license, attribution, transformations, and size.
- [ ] Prepare and optimize the image assets; verify formats and file sizes.
- [ ] Keep the current licensed model as fallback if no suitable generic source is usable.

### Task 2: Redesign the hero and 3D stage
**Files:**
- Modify: `index.html`
- Modify: `dist/index.html`

- [ ] Rework hero composition around one concise Arabic headline, dominant vehicle, restrained navigation, clear primary booking/explore action.
- [ ] Load the unbranded coupe with a local asset URL, delayed loading, and a visually composed fallback.
- [ ] Tune the camera, floor, lighting, and hit regions for six service areas.
- [ ] Verify each service focuses on its intended area and the back control restores the full car.

### Task 3: Build service story and booking flow
**Files:**
- Modify: `index.html`
- Modify: `dist/index.html`

- [ ] Replace repetitive feature-card rhythm with distinct exterior, detail-protection, and interior chapters using relevant generated/verified visuals.
- [ ] Keep service descriptions factual, route each CTA to the correct WhatsApp prefilled message, and preserve all six services.

### Task 4: Mobile, motion, and accessibility
**Files:**
- Modify: `index.html`
- Modify: `dist/index.html`

- [ ] Fit 390 px and 360 px widths without document overflow; keep touch targets at least 44 px.
- [ ] Confirm the horizontal service ribbon snaps to the selected service and remains keyboard usable.
- [ ] Respect reduced motion and verify fallback if WebGL is unavailable.

### Task 5: Publish and inspect
- [ ] Confirm root and dist HTML are identical and JavaScript parses.
- [ ] Inspect desktop and phone screenshots; verify hero load, service focus, return, and WhatsApp links.
- [ ] Merge the feature branch to main and confirm the deployed GitHub Pages version.
