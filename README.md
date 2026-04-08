# Locus — Deep Work Studio

> A minimalist lofi Pomodoro timer with ambient soundscapes, session tracking, and customizable focus themes. Built with pure HTML, CSS, and JavaScript — zero dependencies.

**Live demo:** https://taras-polishchuk.github.io/locus/

---

## Features

- **Pomodoro timer** — Focus / Short Break / Long Break sessions, configurable duration
- **Session progress** — Visual dot tracker across the current Pomodoro cycle
- **SVG ring animation** — Smooth circular progress indicator that updates every second
- **Ambient sounds** — Web Audio API–generated soundscapes (rain, forest, etc.) to aid focus
- **Color themes** — Default (purple), Rain (blue), Sunset (orange), Forest (green)
- **Stats panel** — Tracks completed sessions, total focus time, and current streak
- **Desktop notifications** — Browser Notification API alerts when a session ends
- **Settings panel** — Adjust focus/break durations with live preview
- **Fully keyboard accessible** — All controls reachable via keyboard

## Tech stack

| Layer | Detail |
|-------|--------|
| Markup | Semantic HTML5 |
| Styles | CSS custom properties, CSS animations, responsive grid |
| Logic | Vanilla JavaScript (ES6+) |
| Audio | Web Audio API — procedurally generated ambient sounds, no external files |
| Fonts | DM Serif Display, DM Mono, DM Sans (Google Fonts) |

## Project structure

```
locus/
└── index.html    # entire app — styles + markup + JS in one file
```

## How to run

Just open `index.html` in any modern browser. No build step, no server required.

```bash
open index.html        # macOS
xdg-open index.html    # Linux
```

## How it works

1. Choose a session mode — **Focus**, **Short Break**, or **Long Break**
2. Press **Start** — the ring animates down as time passes
3. On session end the browser fires a desktop notification (if permission granted) and auto-advances to the next phase
4. Toggle ambient sound from the sound panel to mask distractions
5. View today's stats in the stats panel at the bottom

## Motivation

Built to explore the Web Audio API without any external libraries and to practice creating a production-quality single-file app with clean CSS architecture.
