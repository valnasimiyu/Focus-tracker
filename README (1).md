# Focus Log

A lightweight, local-first focus tracker for building consistent study/coding habits — no backend, no build step, no dependencies. Just one self-contained HTML file.

Built around a simple idea: distraction habits (phone, social media) are best fought with friction, not willpower. Focus Log tracks a small daily checklist, gives you a built-in Pomodoro timer, and visualizes your streak as a git-log-style commit graph.

## Features

- **Daily habit checklist** — three default habits aimed at distraction:
  - Phone in another room during a study/coding block
  - Completed at least one 25-minute focus session
  - No social media until the first session is done
- **Commit graph** — a 14-day streak view styled like `git log --graph`. Each day is a node: filled when every habit is checked, a partial ring when some are, empty when none are.
- **Built-in Pomodoro timer** — 25-minute focus / 5-minute break cycle with start, pause, reset, and mode switching.
- **Persistent, private, local** — all data is saved to your browser's `localStorage`. Nothing leaves your device, no account needed.

## Tech stack

Plain HTML, CSS, and vanilla JavaScript. No frameworks, no build tooling, no npm install.

## Usage

Just open `index.html` in a browser — locally or hosted anywhere static files are served (GitHub Pages, Netlify, a simple local file open all work).

```bash
git clone https://github.com/<valnasimiyu>/<Focus-tracker>.git
cd <Focus-tracker>
open index.html   # or just double-click it
```

To host it on GitHub Pages: Settings → Pages → deploy from the branch containing `index.html`.

## Customizing

The default three habits live in the `DEFAULT_HABITS` array near the top of the `<script>` block — edit that array to track whatever habits matter to you. Timer length (25/5 min) is set in the `timerSeconds` logic and can be adjusted the same way.

## License

MIT — use it, fork it, change it.
