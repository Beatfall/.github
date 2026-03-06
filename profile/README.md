# Beatfall

Browser-based rhythm games where your performance shapes the music.

## Repositories

| Repo | Description | Visibility |
|------|-------------|------------|
| [beatfall](https://github.com/Beatfall/beatfall) | Orchestrator — ties all components together via git submodules | private |
| [beatfall-game](https://github.com/Beatfall/beatfall-game) | Main game integrating all Beatfall components into a cohesive cooperative music experience | private |
| [beatfall-sync](https://github.com/Beatfall/beatfall-sync) | Real-time multiplayer music composition synchronization engine | private |
| [beatfall-audio](https://github.com/Beatfall/beatfall-audio) | Music assets, sound effects, audio processing tools, and metadata-tagged audio library | private |
| [beatfall-art](https://github.com/Beatfall/beatfall-art) | Concept art, visual design assets, style guides, and art direction | private |
| [beatfall-prototypes](https://github.com/Beatfall/beatfall-prototypes) | Rapid gameplay prototypes — from one-shot experiments to validated concepts | private |
| [beatfall-research](https://github.com/Beatfall/beatfall-research) | Research papers, design documents, terminology glossary, and reference materials | private |

## What we're building

**Beatfall** is a browser rhythm game built on the Web Audio API. Every hit, miss, and combo shapes the music in real time. At the end of each session the game exports a personalized WAV remix of your performance.

The stack is intentionally minimal: vanilla TypeScript, Canvas 2D, no framework. Audio reactivity runs on `AudioContext` + `AnalyserNode`; procedural beats mean you can play with zero audio assets.

**beatfall-sync** is the multiplayer layer — a real-time event sync engine with latency compensation, session management, and state snapshots for shared musical performances.

## Tech

- TypeScript (strict) · Vite · Canvas 2D · Web Audio API
- WebGL (planned: audio-reactive point cloud background)
- WebSockets · real-time event bus (beatfall-sync)
