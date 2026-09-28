# HyperFrames / HTML+GSAP adapter

Best for agent-native web motion, deterministic UI morphs and loops.

Guidelines:
- use time-addressable/deterministic state where practical
- avoid hidden state that makes frame seeking inconsistent
- centralize style tokens
- prefer SVG/DOM/Canvas based on the visual problem
- GSAP timelines are fine when rendering remains reproducible
- inspect text sharpness during camera scaling
