# Motion Designer v1.4 — Codex Edition

**Motion Designer** is a Codex-first AI-native motion production system.

> 🇵🇱 Wersja polska: [`README.pl.md`](README.pl.md)

`brief → repo inspection → Creative DNA → references → Style Lock → storyboard → patterns → engine router → build → preview → review/fix → export`

## What changed in v1.4
- Codex runtime workflow instead of planning-only behavior.
- Renderer-neutral `motion-project.json` contract.
- Dedicated build skill with repo inspection and preview rules.
- Dedicated audio/beat skill.
- Studio visual defaults kept separate from generic engine rules.
- Machine-readable schemas and starter style profiles.
- Clear adapter contracts for Remotion, HyperFrames, Motion Canvas, Three.js and FFmpeg.
- Bounded review loop with concrete patches.

## Typical usage

```text
/motion Make a 15-second 9:16 launch reel from this app repo.
```

```text
/motion-style Give me three directions for this product. Keep it premium, visual-first and not generic AI-looking.
```

```text
/motion-build Implement the approved storyboard using the best local code-native stack. Render a low-res preview first.
```

```text
/motion-review Review the render and patch blocking visual/timing issues.
```

## Runtime principle
The plugin does not require one renderer. The Motion Project is the source of truth; engines are adapters.

## Repository layout

```text
plugin.json                     plugin manifest
.codex-plugin/plugin.json       Codex interface manifest
AGENTS.md                       operating rules
skills/
  motion-director/              orchestrator, schemas, studio defaults
  motion-style-engine/          style profiles and style library
  reference-scout/              reference gathering
  storyboard/                   timed storyboard authoring
  engine-router/                renderer selection
  motion-build/                 per-engine implementation guides
  audio-design/                 beat/sound design
  motion-reviewer/              visual QA and fix loop
```

## Safety model
- No API keys, tokens, cookies, private client assets or personal data are stored in tracked files.
- Planning and prompts do not authorize paid generation; costs are verified and approved first.
- Renders, previews and uploads are only reported as done when a command actually completed them.

## License
MIT — see [`LICENSE`](LICENSE).

## Third-party notices
Engines and referenced projects keep their own terms — see [`THIRD_PARTY_NOTICES.md`](THIRD_PARTY_NOTICES.md).

## Author
Tabasco Creatives / AI Evolution Labs.
