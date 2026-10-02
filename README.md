# What We Carry: DSS Legacy Walk app

Static mobile web app for the Living Legacy Walk (20 January). No build step.

- `index.html`: the app (GPS stop detection, audio per stop, question prompts, walking music, alerts)
- `sw.js`, `manifest.webmanifest`: offline cache and "Add to Home Screen"
- `audio/`: the six v3 walk tracks, a lo-fi walking loop and the arrival bowl
- `img/`: DSS mark and app icons

## Deploy
Push to GitHub and import in Vercel (framework: Other, no build command, output directory: root).

## Calibrate the stops
Open `/?calibrate` on the test walk. At each stop tap "Set this stop here", then "Copy list" and update the `lat`/`lon` values in `STOPS` in index.html. Coordinates are approximate until then.
