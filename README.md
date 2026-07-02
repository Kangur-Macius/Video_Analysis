# Match Day Analysis

A pitch-side football match analysis app — settings/fixture setup, team analysis, and
individual player tracking with a saveable report. Built as a installable PWA (Progressive
Web App) so it works fully offline on a tablet once added to the home screen.

## Hosting on GitHub Pages

1. Create a new GitHub repository and upload all the files in this folder to the
   repository root (`index.html`, `manifest.json`, `service-worker.js`, the icon PNGs).
2. In the repo, go to **Settings → Pages**, set the source branch (e.g. `main`) and
   folder (`/root`), then save.
3. GitHub will give you a URL like `https://<username>.github.io/<repo-name>/`.

## Installing on your tablet

1. Open that URL in Safari (iPad) or Chrome (Android) **once**, while online.
2. Use "Add to Home Screen" (Safari: Share → Add to Home Screen; Chrome: menu →
   Install app / Add to Home screen).
3. From then on, launch it from the home screen icon — it will open full-screen with
   no browser address bar, and will work with **no internet connection**, since the
   service worker caches everything needed on first load.

## Files

- `index.html` — the entire app (markup, styles, and logic in one file)
- `manifest.json` — PWA metadata (name, icons, colors, display mode)
- `service-worker.js` — caches the app shell so it loads with zero network requests
- `icon-192.png`, `icon-512.png`, `apple-touch-icon.png` — home screen icons
