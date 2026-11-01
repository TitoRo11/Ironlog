# IRONLOG V3

A private, local-first workout tracker PWA for iPhone and desktop.

## Deploy with GitHub Pages

Upload the contents of this folder to the root of the existing `Ironlog` repository, replacing the existing files, then commit to `main`. GitHub Pages should use `main` and `/(root)`.

## Install on iPhone

Open the published GitHub Pages URL in Safari, tap Share → Add to Home Screen. Choose Open as Web App if offered.

## Data and backups

Workout data remains in browser `localStorage` under the existing `ironlog-v1` key. This update deliberately retains that key and migrates older sets by adding `warmup: false` where missing. The service worker cache is separate from workout data. Export JSON backups regularly; clearing Safari website data can erase local workouts.

## V3 features

- Dual-axis exercise progression chart: reps on the left, kg on the right, by workout date.
- Graph periods: 1m, 3m, 6m, 1y, all time.
- Progress filters for exercise, workout/session, and muscle group.
- Last/Best performance comparison in the workout editor.
- Rules-based progressive-overload guidance that considers exercise order/fatigue and exercise category.
- Exercise search picker with a scrollable result area.
- Clickable workout history with workout renaming and copy-to-new-workout.
- Warm-up set markers, excluded from PRs and progression charting.
- Home-screen PR achievement links to exercise progress.
- Offline app shell and network-first page navigation.

No workout data is uploaded to GitHub Pages. The coaching recommendation is a local heuristic, not a cloud AI service or medical advice.
