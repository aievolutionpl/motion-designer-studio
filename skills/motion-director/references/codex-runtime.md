# Codex runtime workflow

## Inspect first
Check the current repo before adding dependencies. Prefer the existing package manager in this order: lockfile evidence first, then package metadata.

Look for:
- `package.json`, `pnpm-lock.yaml`, `yarn.lock`, `bun.lock*`, `package-lock.json`
- existing `remotion`, `three`, `gsap`, `motion-canvas`, `ffmpeg` scripts
- design tokens, fonts, images, screenshots and reusable product UI

## Workspace placement
Prefer:
1. an existing video/motion folder if present,
2. otherwise `motion/` at repo root.

Avoid mixing generated render files into application source.

Recommended:
```text
motion/
  motion-project.json
  src/
  assets/
  previews/
  output/
  notes/
```

## Installation
Do not globally install dependencies. If a requested build requires missing local packages, use the repo's existing package manager and add only the minimum dependencies. Preserve existing versions when possible.

## Preview-first
Before a full-quality render:
1. validate the composition,
2. render representative still frames,
3. render a short/low-res preview,
4. inspect output,
5. patch issues,
6. only then produce final output.

## Validation
Run the smallest relevant checks: typecheck/lint/build for touched code. Do not run unrelated destructive scripts.
