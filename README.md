# Tri-Calendar PWA · বাংলা · English · হিজরি

Offline-capable Progressive Web App: convert dates between Gregorian, Bangla (Bangladesh revised) and Hijri calendars.

## Files
| File | Purpose |
|---|---|
| `index.html` | App (HTML + CSS + JS, single file) |
| `manifest.webmanifest` | Install metadata (name, icons, theme) |
| `sw.js` | Service worker: offline cache |
| `icons/` | 192, 512, maskable 512, Apple touch icon, SVG favicon |

## Run locally
Service workers need HTTP(S) (not `file://`):
```
python3 -m http.server 8080
```
Open http://localhost:8080

## Deploy (HTTPS required)
- **GitHub Pages:** push the folder → Settings → Pages.
- **Netlify / Vercel / Cloudflare Pages:** drag-and-drop the folder.
- Works in a sub-folder too (all paths are relative).

## Install
- **Android/Chrome:** menu → Install app.
- **iOS/Safari:** Share → Add to Home Screen.
- **Desktop Chrome/Edge:** install icon in the address bar.

## Updating
Edit files, then bump `VERSION` in `sw.js` (e.g. `v2`) so users receive the new cache.
