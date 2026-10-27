# Gym Attendance Tracker (PWA)

A mobile-first monthly gym attendance calendar. The app uses localStorage, supports JSON backup/restore and CSV export, and caches its app shell for offline use after the first successful visit.

## Deploy using only an Android phone

1. Sign in to GitHub in Chrome and create a **public** repository named `gym-attendance`.
2. Upload the files and folders in this project, keeping the structure exactly as shown (`index.html`, `manifest.webmanifest`, `service-worker.js`, `icons/`).
3. In the repository, open **Settings → Pages**. Choose **Deploy from a branch**, select `main` and `/(root)`, then Save.
4. Wait for GitHub Pages to publish. The site URL is normally `https://YOUR-USERNAME.github.io/gym-attendance/`.
5. Open the URL in Android Chrome and let it load once while online. Allow a moment for the service worker to cache the app shell.
6. In Chrome's ⋮ menu choose **Install app** or **Add to Home screen**. The wording can differ by Chrome version.
7. Launch from the home-screen icon. Try Airplane mode to confirm the interface opens offline.

GitHub Pages setup labels can change. Do not upload passwords, tokens, or private data to the repository.

## Files

- `index.html`: user interface and calendar logic
- `manifest.webmanifest`: installable PWA metadata
- `service-worker.js`: offline application-shell cache
- `icons/icon-192.png`, `icons/icon-512.png`: app icons

## Data safety

Attendance records stay in this browser's localStorage. Export a JSON backup periodically. Clearing Chrome site data or changing browser/device can remove or leave behind the data; import the backup to restore it. This app does not send attendance data to a server.
