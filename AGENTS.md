# Motion Designer — Codex operating rules

This is a Codex-first motion-production plugin. The main owner is `skills/motion-director/SKILL.md`.

## Activation
Use this plugin for launch videos, UI motion, kinetic type, explainers, product films, social reels, logo motion, motion systems, coded video and review/fix work.

## Core behavior
1. Inspect the current repository before proposing a stack.
2. Reuse the existing package manager and framework where practical.
3. Keep a renderer-neutral Motion Project as source of truth.
4. Establish Creative DNA and Style Lock before non-trivial scene implementation.
5. Storyboard before building a multi-scene film.
6. Prefer deterministic local/code-native motion when it can match the brief.
7. Treat generated video as a shot asset, not the master timeline.
8. Build low-cost previews before final renders.
9. Review actual frames/output before calling a video finished.
10. Limit autonomous review/fix loops to three cycles unless blocking defects remain.

## Repository safety
Do not rewrite the host app architecture just to add a video. Prefer an isolated `motion/` workspace or an existing video directory. Do not delete user files or replace existing dependencies without need. Never put API keys, tokens, cookies, private client assets or personal data into tracked plugin/project files.

## Paid/external generation
Planning, prompts and code do not authorize paid generation. Before any paid external call, verify current provider/model parameters and cost using the available provider tool and obtain whatever approval that tool requires.

## Truthfulness
Never claim a render, preview, install, generation, upload or deployment completed unless a tool/command actually completed it. If a renderer is unavailable, produce the exact implementation/adaptor plan instead of faking execution.
