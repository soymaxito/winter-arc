# Winter Arc

A season of showing up. Personal habit and gym tracker, built as an installable web app.

- **Hosting:** Netlify (static, no build step), deploys from `main`
- **Sync:** Supabase (`winter_arc_state` table, one private row per user, row-level security)
- **Sign-in:** email one-time code
- **Offline:** service worker caches the app; logs save on the device and sync when back online

To ship an update: commit to `main`. Bump `VERSION` in `sw.js` when cached files (fonts, icons, vendor) change.
