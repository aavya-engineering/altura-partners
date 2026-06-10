# Altura Partners — Landing Page

Static single-page site for Altura Partners, an early-stage venture fund
(AI · Semiconductors · Physical AI · Space · Defense). Reproduced from the
provided design with an added light/dark theme toggle.

## Files
- `index.html` — markup
- `styles.css` — styles (dark default + light theme under `html[data-theme="light"]`)

No build step. Pure HTML/CSS + a tiny inline JS for the theme toggle.

## Run locally
Open `index.html` in any browser, or serve the folder:
```
python -m http.server 8000
```

## Theme toggle
Sun/moon button in the nav. Choice is saved to `localStorage`
(`altura-theme`). Defaults to dark (the original design).

## Deploy — GitHub Pages
1. Create a new repo on GitHub (e.g. `altura-partners`).
2. From this folder:
   ```
   git remote add origin https://github.com/<you>/altura-partners.git
   git push -u origin main
   ```
3. Repo → Settings → Pages → Source: `Deploy from a branch`,
   Branch: `main` / `/ (root)` → Save.
4. Live at `https://<you>.github.io/altura-partners/` within a minute or two.
