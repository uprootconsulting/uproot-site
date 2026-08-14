# Uproot Consulting — Website (V7)

Static site. No build step. Deploys as-is on Netlify.

## Structure
- `index.html` — Home (hero, 三個處境, offers overview, how we work, Soul Code teaser, CTA)
- `services/` `how-we-work/` `case-study/` `about/` `contact/` — one folder per page (clean URLs)
- `assets/` — `style.css` (shared), `logo.png` (transparent), `pak.jpg`
- `_redirects` — old site URLs (/consultation, /service, /courses) → new pages

## Deploy (GitHub → Netlify)
1. github.com → New repository → name e.g. `uproot-site` (Private OK) → Create
2. In the repo: **Add file → Upload files** → drag ALL files & folders in this package → Commit
3. Netlify → open your EXISTING site (keeps the domain) → Site configuration → Build & deploy → **Link repository** → GitHub → pick `uproot-site`
4. Build command: (leave empty) · Publish directory: `/` → Save
5. Future edits: upload changed files on GitHub → Netlify auto-deploys in ~30s
