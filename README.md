# marendych.github.io

Landing pages + Apple App Site Association (AASA) for **Corio** iOS app.

## What's here

- `.well-known/apple-app-site-association` — AASA file for iOS Universal Links (`/invite/*`, `/profile/*` paths open Corio directly when installed).
- `404.html` — universal landing that:
  - matches `/profile/:username` and `/invite/:code`
  - tries to open `forma://...` deep link
  - falls back to App Store on iOS if app isn't installed
  - shows generic CTA on desktop / Android
- `index.html` — root, redirects to App Store.

## Test URLs (after publish)

- https://marendych.github.io/ → App Store
- https://marendych.github.io/profile/aliona → profile landing
- https://marendych.github.io/invite/ABC123 → invite landing
- https://marendych.github.io/.well-known/apple-app-site-association → AASA JSON
