# ONE K Studio — design direction
**Date:** 2026-10-24  
**Status:** Approved direction  
**Repository:** gmloj/one-k-auto

## Goal
Make ONE K feel like a premium car-care studio and let the vehicle remain the center of service discovery. The page should help visitors understand six care services and contact the shop through WhatsApp.

## Direction
- Keep the dark graphite/orange identity and current 3D showroom, including the newest mobile service dock.
- Add cinema through composition, light, depth, type, and transitions in the existing Three.js scene; avoid heavy autoplay video and large decorative downloads.
- Present a concise Arabic hero, clear exploration and booking actions, and editorially styled service sections.
- Add an optional service-category filter: all (6), exterior (4), interior (2), with accessible pressed states.
- Keep current Arabic descriptions and WhatsApp links. Do not invent prices, guarantees, customer stories, statistics, or performance claims.
- The car asset stays transparently attributed to its creator; hide only visible logo or badge meshes when their names are identifiable, without hiding functional vehicle geometry.
- Preserve mobile-first layout, all six service controls, the 3D focus/return behavior, reduced-motion support, and root/dist parity.

## Scope
Modify root `index.html` and `dist/index.html`. No database, checkout, account, or new tracking systems.
