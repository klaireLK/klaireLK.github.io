# Portfolio — Hyacinth Klaire E. Manzano

Single-file portfolio website for a data clerk. Clean, minimal, responsive — built with plain HTML/CSS/JS.

## One file

```
index.html     ← everything (HTML, CSS, JS inline)
```

Open `index.html` in a browser — that's it.

## Customize

| What | Where in `index.html` |
|------|----------------------|
| Name / title / tagline | Hero section (search `#hero`) |
| Stats numbers | Stats section — `data-target` attributes |
| Skills | Skills section — 4 cards with inline SVGs |
| Process steps | Process section — 4-step strip |
| Work examples | Featured work section — 2 cards |
| Testimonial | Testimonial section — switch quote + attribution |
| Certifications | Certifications section — pill badges |
| Email / LinkedIn | Contact section |
| Resume file | Replace `resume.pdf` (or update link) |

## Deploy on GitHub Pages

```bash
git add index.html README.md
git commit -m "Update portfolio"
git push origin main
```

Then in your repo: **Settings → Pages → branch `main`, folder `/ (root)`** → Save. Site goes live in ~2 minutes.
