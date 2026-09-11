COST WALK STUDIO - offline PWA for iPhone
=========================================

Files: index.html, manifest.json, sw.js, icon-192.png, icon-512.png, apple-touch-icon.png

DEPLOY (GitHub Pages, same as your other apps):
1. Create a repo (e.g. costwalk-app) under your GitHub account.
2. Upload ALL six files to the repo root (drag-and-drop on github.com works).
3. Settings -> Pages -> Deploy from branch -> main / root -> Save.
4. Open https://<username>.github.io/costwalk-app/ in Safari on the iPhone.
5. Share -> Add to Home Screen. Open it once from the Home Screen while online
   so the service worker caches everything - after that it works fully offline.

DATA:
- Autosaves to the device (localStorage) on every change.
- Export gives a JSON backup file; Import merges it back on any device.
- Because iOS ties storage to the app icon, take an occasional Export backup.
