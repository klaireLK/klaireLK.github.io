# Portfolio — Hyacinth Klaire E. Manzano

A clean, responsive personal portfolio website built with plain HTML, CSS, and JavaScript. Ready to deploy on GitHub Pages in one click.

## Project Structure

```
├── index.html          # All page content (hero, about, skills, projects, contact)
├── css/
│   └── style.css       # All styles — colors, layout, responsive
├── js/
│   └── main.js         # Mobile menu toggle & smooth scrolling
├── assets/
│   └── profile.jpg     # Replace with your photo
└── README.md
```

## Customization Guide

### 1. Replace your name & tagline
Open `index.html`. Find these lines near the top of `<section id="hero">`:

- **Line ~64:** `<h1>Hyacinth Klaire E. Manzano</h1>` — your name
- **Line ~65:** Tagline inside the `<p class="tagline">` element

### 2. Replace the About bio
In `index.html`, find `<section id="about">`. Replace the two `<p>` paragraphs with your real bio.

### 3. Replace skills
In `index.html`, find `<section id="skills">`. Each `<div class="skill-card"><span>...</span></div>` is one skill. Add, remove, or rename them.

### 4. Replace projects
In `index.html`, find `<section id="projects">`. Each `<article class="project-card">` is one project. Update the title, description, tags, and links. To add more, copy an entire `<article>` block.

### 5. Replace contact info
In `index.html`, find `<section id="contact">`. Update the email address and social links.

### 6. Replace profile photo
Replace `assets/profile.jpg` with your own photo (square works best). Keep the same filename or update the `<img src>` path in `index.html`.

### 7. Customize colors
Open `css/style.css`. The `:root` section at the top defines all colors:

```css
--bg-primary: #1a1a2e;    /* main background */
--bg-secondary: #16213e;  /* alternate section background */
--accent: #00b4d8;        /* accent color (links, borders) */
--accent-hover: #0090b0;  /* accent hover state */
--text: #e0e0e0;          /* body text */
--text-light: #a0a0b0;   /* muted text */
```

## Run Locally

Because this is plain HTML/CSS/JS, you can open it directly:

1. Double-click `index.html` — it opens in your browser.

Or serve it with any static server (optional):

```bash
# Python 3
python -m http.server 8000

# Node (requires npx)
npx serve .
```

Then open `http://localhost:8000` in your browser.

## Deploy to GitHub Pages

This repo is already set up as a GitHub Pages site (`klaireLK.github.io`). To deploy:

1. Push this code to the `main` branch of your GitHub repo:

```bash
git add .
git commit -m "Initial portfolio"
git push origin main
```

2. Go to your repo on GitHub: `https://github.com/klaireLK/klaireLK.github.io`

3. Click **Settings** → **Pages** (in the left sidebar).

4. Under **Source**, select **Deploy from a branch**.

5. Set **Branch** to `main` and folder to `/ (root)`.

6. Click **Save**.

7. Wait 1–2 minutes, then visit `https://klaireLK.github.io` — your site is live.

Any future push to `main` will automatically redeploy.

## License

MIT
