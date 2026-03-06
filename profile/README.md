# Beatfall

Browser-based rhythm games where your performance shapes the music.

## Repositories

| Repo | Description |
|------|-------------|
| [beatfall](https://github.com/mroncka/beatfall) | Rhythm game client — Web Audio API, Canvas 2D, TypeScript |
| [beatfall-sync](https://github.com/Beatfall/beatfall-sync) | Real-time multiplayer synchronization engine |

## What we're building

**Beatfall** is a browser rhythm game built on the Web Audio API. Every hit, miss, and combo shapes the music in real time. At the end of each session the game exports a personalized WAV remix of your performance.

The stack is intentionally minimal: vanilla TypeScript, Canvas 2D, no framework. Audio reactivity runs on `AudioContext` + `AnalyserNode`; procedural beats mean you can play with zero audio assets.

**beatfall-sync** is the multiplayer layer — a real-time event sync engine with latency compensation, session management, and state snapshots for shared musical performances.

## Tech

- TypeScript (strict) · Vite · Canvas 2D · Web Audio API
- WebGL (planned: audio-reactive point cloud background)
- WebSockets · real-time event bus (beatfall-sync)
