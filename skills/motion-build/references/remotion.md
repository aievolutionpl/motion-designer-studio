# Remotion adapter

Use when the host is React-friendly or the project needs reusable compositions, captions, data and multi-format output.

Guidelines:
- one composition root per output family
- derive animation from frame/time, not wall-clock timers
- use reusable scene/pattern components
- expose dimensions/fps/duration as project config
- keep brand/style tokens centralized
- render still frames before long final renders
- recompose layout for each aspect ratio
