# Portfolio Website Design

## Overview
Personal portfolio website for Hyacinth Klaire E. Manzano, deployed via GitHub Pages. Single-page scroll with smooth anchor navigation.

## Tech Stack
- Plain HTML5, CSS3, JavaScript (zero dependencies)
- No build step — deploy by pushing to GitHub

## Site Structure
1. **Hero** — Full viewport intro with name, tagline, profile photo placeholder, CTA button
2. **About** — Short bio placeholder paragraph
3. **Skills** — Responsive grid of skill cards (9 placeholder skills)
4. **Projects** — 3 project cards (title, description, tech tags, links)
5. **Contact** — Email + GitHub + LinkedIn links
6. **Footer** — Copyright line

## Design
- **Colors:** Deep navy (#1a1a2e) background, teal (#00b4d8) accent, light gray text
- **Typography:** System font stack
- **Layout:** CSS Grid/Flexbox, fully responsive
- **Mobile:** Hamburger menu, stacked single-column layout below 768px

## File Structure
```
/
├── index.html
├── css/style.css
├── js/main.js
├── assets/profile.svg
├── docs/superpowers/specs/2026-07-09-portfolio-website-design.md
└── README.md
```

## Key Design Decisions
- Plain HTML/CSS/JS chosen over Jekyll/Astro for zero build step, fastest deploy, and easiest customization for a beginner
- SVG placeholder used for profile photo instead of real image
- All content in single HTML file for simplicity
- CSS custom properties for easy theming
