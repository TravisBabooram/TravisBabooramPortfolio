# Travis Babooram — Portfolio

Single-file animated portfolio. Zero build step, zero npm dependencies — one `index.html` containing hand-written HTML/CSS/JS, GSAP (via CDN) and a hand-rolled WebGL nebula shader.

## Run locally
Any of these, from this folder:

- **VS Code Live Server** (recommended): install the prompted extension, then click **Go Live** in the status bar — auto-reloads on save.
- `python3 -m http.server 8000` → http://localhost:8000
- `npx serve`

Opening `index.html` directly also works, but serving over http is more faithful (fonts/CORS).

## Deploy
Pure static: drag the folder into Netlify Drop, import to Vercel, or push to GitHub Pages. Then point a custom domain at it.

## Test checklist (after any change)
- Preloader → hero intro → click shockwave → pinned gallery → terminal (`help`)
- Narrow viewport (<900px): vertical gallery, no custom cursor/tilt
- DevTools → emulate `prefers-reduced-motion`: theatrics off, content intact
- Block cdnjs in DevTools: page still readable
