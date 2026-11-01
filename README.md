# ACCT689 Exam Prep Quiz

Static quiz app (index.html). No build step, no dependencies. Works on phone and laptop, can be installed as an app, and works offline after the first visit. Progress is saved in the browser (localStorage) of each device.

## Files
- `index.html`: the app (slides, styles and code)
- `manifest.webmanifest`: app name, colours, icons and full-screen setting
- `sw.js`: service worker that makes the app installable and usable offline
- `icon-192.png`, `icon-512.png`, `icon-maskable-512.png`, `apple-touch-icon.png`, `favicon-32.png`: app icons
- `vercel.json`: clean URLs and cache headers
- `package.json`, `README.md`

Keep every file at the repo root.

## Deploy to Vercel via GitHub
1. Upload ALL files in this folder to the GitHub repository (replace the old ones).
2. Vercel redeploys automatically. For a new project: Add New Project → Import the repo → Framework preset "Other" → leave Build Command and Output Directory empty → Deploy.
3. Install on your phone:
   - iPhone: open the site in Safari → Share → Add to Home Screen.
   - Android: open in Chrome → tap "Install app" (in the top bar or the ⋮ menu).

## Updating content
Edit index.html and push. When you change sw.js or the icons, bump `VERSION` in sw.js so installed apps pick up the new files.
