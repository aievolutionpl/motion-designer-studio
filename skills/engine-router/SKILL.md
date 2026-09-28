---
name: engine-router
description: Route each motion scene to the simplest capable local engine, considering current repo stack, required quality, cost and runtime availability.
---

# Engine Router

Default to `engine=auto`.

Read `references/routing.md` and the current repo inspection before deciding.

Prefer:
- HyperFrames/HTML+GSAP for deterministic UI morphs, loops and procedural web-native scenes.
- Remotion for React composition, reusable templates, captions, dynamic data and multi-format social output.
- Motion Canvas for diagrams, explainers and vector-heavy technical motion.
- Three.js for spatial/3D product scenes.
- After Effects only when available and its compositing/expression capabilities are genuinely needed.
- Generative video for people, lifestyle, environments or impossible footage; treat as shot assets.
- FFmpeg for final assembly, audio, transcode and delivery.

## Routing rule
Choose the lowest-complexity engine that meets the acceptance criteria. Avoid mixing engines unless the visual gain justifies integration cost.

## Cost modes
Quality / Balanced / Budget. Never invent live external pricing.
