# NewbieGym 💪

**From Zero to Strong — Gym & Calisthenics Tracker**

A beginner-friendly **hybrid workout tracker** (barbell/dumbbell/machine training **and** bodyweight calisthenics) in a single HTML file. Remade & upgraded from the spirit of [OpenGym](https://github.com/alexpcosta/opengym) — but zero-backend, zero-dependency, and designed mobile-first to be wrapped into an Android APK with Capacitor/WebView.

## Features

- **Home** — greeting hero with weekly streak (🔥), total workouts, lifetime volume, and a gamified **Level/XP bar** (Level 1 *Newbie* → Level 5 *Intermediate*), a consistency calendar, quick start, and 4 pre-built beginner routines (Gym Full Body, Calisthenics Foundation, Hybrid Upper, Hybrid Lower).
- **Workout Logger** — three tracking types that adapt per exercise:
  - *Weight + Reps* (gym), *Bodyweight + added kg + Reps* (calisthenics), *Timed Holds* with a built-in stopwatch (plank, L-sit, dead hang).
  - Set-type badges (working / **W** warm-up / **F** failure), last-performance hints, PR detection on finish, XP rewards.
  - **Auto rest timer** (floating bar, ±15s / skip, Web Audio beep + vibration) that starts when you check a set. The session clock is timestamp-based, so it stays accurate when the screen locks.
- **Exercises** — 28 pre-loaded gym & calisthenics movements with **Newbie Form Cues** (step-by-step injury-prevention tips) and calisthenics **Progression Paths** (e.g. Knee Push-up → Push-up → Diamond → Archer). Filter by category/muscle, search, and add unlimited **custom exercises**.
- **Tools** — 1RM calculator (Epley formula, with % table) and a visual **barbell plate calculator** (20 kg bar).
- **Progress** — weekly volume chart, calisthenics max-reps/hold progression line, personal bests, body-weight tracker with BMI and beginner calorie/protein targets, full workout history.
- **100% Offline** — everything is stored in `localStorage`, with **Export / Import backup (.json)** so your data survives an APK reinstall.

## Tech

- Single file: `index.html` (HTML + CSS + vanilla JS). No build step, no CDNs, no backend — it works from `file://`, any static host, or inside a WebView.
- White & Sporty Blue design system (`#F8FAFC` background, `#2563EB` → `#0EA5E9` brand gradient), native-app chrome: fixed top bar, bottom tab navigation, safe-area insets, 48px+ touch targets.

## Run it

Open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```

## Roadmap to APK

Wrap with [Capacitor](https://capacitorjs.com): `npx @capacitor/cli init` and point `webDir` at this folder — the app is already offline-first and touch-optimized.

## License

MIT
