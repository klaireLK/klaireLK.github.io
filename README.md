# Portfolio — Hyacinth Klaire E. Manzano

A modern, responsive personal portfolio built with plain HTML, CSS, and JavaScript. Lightweight, zero dependencies, ready for GitHub Pages.

## Project Structure

```
├── index.html           # All page content
├── css/
│   └── style.css        # Animated gradient hero, glass cards, responsive grid
├── js/
│   └── main.js          # Mobile menu, scroll-triggered fade-in animations
├── assets/
│   └── profile.svg      # Replace with your photo (square works best)
├── docs/                # Design documentation
└── README.md
```

## What's Inside

- **Animated gradient hero** with floating profile photo
- **Glass-morphism cards** for skills and projects
- **Scroll-triggered fade-in animations** via IntersectionObserver
- **SVG section dividers** for visual flow between sections
- **Fully responsive** — mobile, tablet, desktop
- **Single Google Font** (Inter) — clean, professional, fast

## Customization Guide

### 1. Your name & tagline
`index.html` → `<section id="hero">`:
- Line ~61: `<h1>` — your name
- Line ~64: `<p class="tagline">` — short professional tagline

### 2. Bio
`index.html` → `<section id="about">` — replace the two paragraphs.

### 3. Skills
`index.html` → `<section id="skills">` — each `.skill-card` is one skill. Rename, add, or remove them. Each includes an inline SVG icon (swap icons by replacing the `<svg>` inside each card).

### 4. Projects
`index.html` → `<section id="projects">` — each `.project-card` is one project. Update title, description, tags, and links.

### 5. Contact
`index.html` → `<section id="contact">` — update email, GitHub, and LinkedIn URLs.

### 6. Profile photo
Replace `assets/profile.svg` with your actual photo (square, preferably 300×300px). Update the `<img src>` path in `index.html` if you change the filename.

### 7. Colors
Open `css/style.css` — the `:root` section defines the palette:
```css
--bg: #0a0a0f;           /* dark background */
--bg-alt: #111118;       /* alternate section background */
--accent-1: #8B5CF6;     /* purple accent */
--accent-2: #EC4899;     /* pink accent */
--text: #e8e8f0;         /* body text */
--text-muted: #7878a0;   /* muted text */
```

## Run Locally

Simply open `index.html` in your browser. Or serve with any static server:

```bash
# Python 3
python -m http.server 8000

# Node (optional)
npx serve .
```

Then visit `http://localhost:8000`.

## Deploy to GitHub Pages

1. Push to `main`:
```bash
git add .
git commit -m "Update portfolio"
git push origin main
```

2. Go to your repo → **Settings** → **Pages**

3. Set **Source** to **Deploy from a branch**, **Branch** to `main`, **folder** to `/ (root)`, and click **Save**.

4. Wait ~2 minutes, then visit `https://klaireLK.github.io`.

Any push to `main` auto-deploys.

## Design Decisions

- **Plain HTML/CSS/JS** chosen over Jekyll/Astro for zero build step and easiest editing
- **Single-page scroll** avoids layout duplication and feels smooth
- **Content kept general** — skills and projects are placeholders for any profession
- **One Google Font import** (Inter) to keep load fast while improving typography
