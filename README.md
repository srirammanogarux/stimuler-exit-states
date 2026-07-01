# Stimuler — Video-lesson Exit State

An interactive prototype of the **exit-intent bottom sheet** shown when a learner tries to leave
mid-lesson in Stimuler. Instead of just letting them go, the sheet empathises, hands them quick
**controls** to fix whatever's bothering them (video language, playback speed), and quietly captures
**why they're leaving** — turning a churn moment into a "keep going" moment.

**Live demo:** https://exit-states.vercel.app

## The flow
Roadmap → tap **Start exercise** → the video plays → tap **Back** → the exit sheet slides up.

- **Video language** — English / Bahasa
- **Playback speed** — 0.5×–2.0× slider
- **"Leaving already?"** reason chips — picking one turns the primary CTA into **Send report**,
  which acknowledges the feedback and returns you to the lesson
- **Keep learning** (primary) / **End session** (secondary)
- A floating **View code** toggle reveals this prototype's own source

## Tech
A single self-contained `index.html` (no build step). Fonts via Google Fonts (Urbanist).
Frame backgrounds under `assets/` are exported from the Figma design.

Open `index.html` directly, or serve the folder:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

🤖 Prototype built with [Claude Code](https://claude.com/claude-code)
