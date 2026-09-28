---
name: motion-build
description: Implement an approved Motion Project inside the current Codex repo, scaffold an isolated motion workspace, build previews, render with available local tools and keep changes minimal/reviewable.
---

# Motion Build

Use after storyboard/style approval or when the user explicitly asks to build immediately.

## 1. Inspect and choose placement
Use the existing motion/video folder if present; otherwise create `motion/`.

## 2. Preserve the host app
Do not refactor unrelated application code. Reuse brand tokens, product UI and assets through imports/copies that keep the video workspace clear.

## 3. Implement by adapter
Follow Engine Router. Read the relevant adapter reference:
- `references/remotion.md`
- `references/hyperframes.md`
- `references/motion-canvas.md`
- `references/threejs.md`
- `references/ffmpeg.md`

## 4. Preview-first
Before final render:
- render representative scene frames,
- produce a low-res/short preview where possible,
- inspect it,
- run Motion Reviewer,
- patch high-value issues.

## 5. File discipline
Keep generated previews/output out of app source. Use:
`motion/previews/` and `motion/output/`.

## 6. Dependency discipline
Use the repo's package manager. Add only required local dependencies. Do not global-install tools. If FFmpeg is missing, detect and report it rather than claiming assembly succeeded.

## 7. Completion
Report exactly what changed, where the preview/final file is, which engine was used, and what remains unverified.
