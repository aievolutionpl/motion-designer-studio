---
name: motion-director
description: Main Codex orchestrator for motion design. Inspect the repo, create Motion Project IR, Creative DNA, Style Lock, storyboard, engine plan, build/review loop and delivery.
---

# Motion Director

Use this as the default owner for `/motion`.

## Phase 0 — inspect the working repo
Before suggesting a renderer, inspect the project structure and relevant files: package manifest, lockfile, framework, existing assets, fonts, brand tokens, screenshots, README and any existing video/motion code. Do not crawl irrelevant directories.

Determine:
- package manager
- React/Next/Vite/other stack
- existing Remotion/Three.js/GSAP/FFmpeg support
- reusable UI components/assets
- output directory conventions

Read `references/codex-runtime.md`.

## Phase 1 — project contract
Create or update `motion/motion-project.json` from `references/motion-project.schema.json`. This is the renderer-neutral source of truth.

## Phase 2 — creative system
1. Load brand constraints and `references/personal-defaults.md` unless the user supplied stronger direction.
2. Use Reference Scout when references are supplied or external inspiration is needed.
3. Use Motion Style Engine to produce Creative DNA + Style Lock.
4. Build storyboard for any non-trivial multi-scene piece.
5. Select motion patterns.

## Phase 3 — route and build
Use Engine Router. Prefer the simplest engine that can achieve the required quality while fitting the current repo.

Then use `motion-build` to implement.

## Phase 4 — review
Render beat frames or low-res preview first when possible. Use Motion Reviewer on actual output. Patch blocking/high-value issues, maximum three normal cycles.

## Multi-format
Recompose layout per aspect ratio. Never rely on blind crop for 16:9, 9:16, 4:5 and 1:1.

## Stop conditions
Stop and explain if:
- required renderer/tool is unavailable,
- a paid external step requires confirmation,
- a reference/product asset required for fidelity is missing,
- the user asked only for a plan/prompt/storyboard.
