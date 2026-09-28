# Life Sprint — Florida 2-14

A mobile-friendly, dependency-free study app for Florida Life (including Annuities & Variable Contracts).

Open `dist/index.html` in a browser, or serve the `dist` directory using any static web server. No build or API keys required.

Features: original multiple-choice questions with explanations; six topic lessons; a 15-question training round; 20-question / five-minute sprint; 95-question timed boss run; combo rewards and sound effects; mistake review; XP ranks; browser-local progress and session resume.

All rehearsal questions count toward the practice score. The official 2026 exam has 85 scored and 10 unscored questions. This is a focused study aid, not an official exam bank, exhaustive curriculum, or score guarantee. Sources and section weights are linked inside the app. Content checked September 27, 2026.

Progress lives in localStorage on each browser and is not sent to a server. Timed sessions continue while the app is closed. GitHub contains code only, not study progress.

## Arcade update

Every quiz mode now has a per-question timer: Charged (20s, default), Overdrive (15s), or Blitz (10s). A timeout locks the question as incorrect. Feedback is immediate and remains visible until Next, when a fresh timer starts. Sprint additionally retains its five-minute round limit. The 95-question Boss Run is intentionally faster than real exam timing and is not an exam-time simulation.

Correct answers earn base XP plus capped streak and speed bonuses. Wrong answers reset the combo, with a 160ms visual hit stop and brief input lock. Synthesized Web Audio cues start after user interaction. Sound and effects can be toggled; OS reduced-motion is respected. Effects use smooth glows and brief movement, not rapid strobing. Existing ranks and completed history are retained. Legacy unfinished sessions are cleared when migrating to the timed engine.
