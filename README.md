# 🌌 DreamScape AI

A "Life Operating System" dashboard concept — a single self-contained `index.html` with no build step and no backend.

**Live demo:** open `index.html` in any browser, or enable GitHub Pages on this repo (Settings → Pages → Deploy from branch → `main` / root) and it'll be live at `https://<your-username>.github.io/<repo-name>/`.

## What's in it

- **Dream Galaxy** — a 3-year roadmap (Python → ... → Interview Prep) drawn as a constellation from 🌍 to 🪐. Click any star to mark a milestone reached or not.
- **Today's Plan** — an editable daily planner. Add tasks, check them off, delete them. Each task carries XP.
- **Dream Completion ring** — computed live from your roadmap + task progress (60/40 weighted), not hardcoded.
- **Life Balance Radar** — six sliders (Learning, Health, Sleep, Money, Relationships, Mental) that redraw the radar chart as you drag them.
- **Gamification** — XP, levels, titles, and badges that update as you complete things.
- **Future Self** — a typewritten message generated from your current completion % and streak.
- **Dream Weather** — a mood readout (☀️ Momentum / 🌧 Burnout Risk / 🌈 Creative Flow / 🌩 Overloaded) computed from your stats.
- **Time Machine** — a 2026–2030 slider projecting your completion forward at your current pace.
- **Weekly Growth chart** — a simple SVG bar chart.

All state (tasks, milestones, balance sliders, XP) is saved to the browser's `localStorage`, so progress persists across reloads. No data leaves your browser — there's no backend, no API calls, no tracking.

## Tech

Vanilla HTML, CSS, and JavaScript. One font import (Google Fonts: Fraunces, Inter, IBM Plex Mono) — everything else is self-contained.

## Running locally

Just open `index.html` directly, or serve it so relative paths behave consistently:

```bash
npx serve .
# or
python3 -m http.server 8000
```

## Roadmap / not yet built

This is the "flagship slice" of a much bigger product concept (see the original vision doc). Not included yet, and would need a real backend/AI API to do honestly rather than fake it:

- Future Self as a generated video/voice avatar
- A "Regret Simulator" with real predictive modeling
- Multi-user accounts, sync across devices
- The AI Learning / Project Generator / Interview Coach / Resume Builder modules
