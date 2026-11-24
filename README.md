# Transatlantic Relations — study app

Interactive study guide for the Transatlantic Relations midterm (Lectures 1–7): read each section with a plain-English explanation, quiz yourself on that section, flashcards, timeline, exam essay prompts. Progress saves in the browser (localStorage + cookie). Light/dark toggle.

## Files
- `index.html` — the app
- `data.json` — all content, questions and explanations (loaded by the app)
- `Dockerfile` — serves the folder with Caddy on `$PORT` (Railway / any Docker host)

## Deploy
It's a static site — any static host works.
- **Railway:** New project → Deploy from GitHub repo (uses the Dockerfile automatically) → Settings → Networking → Generate domain.
- **Netlify / Vercel / Cloudflare Pages / GitHub Pages:** upload or point at this folder, no build step, publish directory = root.
- **Local:** `python3 -m http.server 8000` then open http://localhost:8000 (opening index.html directly from disk won't load data.json).
