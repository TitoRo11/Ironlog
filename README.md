# IRONLOG — personal workout tracker

A mobile-first Progressive Web App (PWA) for strength training.

## Files
- `index.html` — app interface and workout logging logic
- `manifest.json` — installable PWA metadata
- `sw.js` — basic offline app-shell cache
- `icon-192.png`, `icon-512.png` — app icons

## Publish with GitHub Pages
1. Create a GitHub account and a **public** repository, e.g. `ironlog`.
2. Upload all five files from this folder to the repository root.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Choose branch `main`, folder `/(root)`, then Save.
6. Wait for the Pages URL shown there, usually `https://YOURNAME.github.io/ironlog/`.

## Install on iPhone
1. Open the published URL in Safari (not an in-app browser).
2. Tap Share → Add to Home Screen.
3. If shown, enable **Open as Web App**, then tap Add.
4. Launch IRONLOG from its new Home Screen icon.

## Data and privacy
Workout records are stored in browser localStorage on the device/browser where you use the app. The GitHub Pages site serves the app files; it does not receive workout records. Export a JSON backup regularly from Exercises → Data & backup. Import a previous JSON backup to restore it. Do not clear Safari website data unless you have a backup.

This first version has no account or cloud sync. Data does not automatically move between devices. It is a client-side app; the GitHub repository contains the app source, not your logged workout data.

## Current features
- Exercise library with common strength exercises and custom exercises
- Session logging with sets, reps, weight, completed-set toggles
- Previous recorded sets shown when adding an exercise; prefilled from last session
- Workout notes
- Personal best recorded weight by exercise
- Progress chart of best recorded weight per session
- Rest timer
- Session history and volume totals
- JSON export/import backup
- Basic offline app-shell caching after first online load

## Important limitations / next improvements
- Records are stored per browser origin and device; use export/import backups.
- This is a starter version. It does not yet include cloud sync, bodyweight tracking, exercise editing/deletion, estimated 1RM, or richer analytics.
- The app uses kilograms as its displayed weight unit.
