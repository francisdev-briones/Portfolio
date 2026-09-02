# Francis.dev — Personal Portfolio (Prelim Project)

A static, responsive personal portfolio website built for the Software Engineering Prelim requirement (BSIT C, 3rd Year). It showcases my background, skills, projects, and certifications in a single-page, dark-themed layout with a canvas-based animated hero background and scroll-triggered reveal animations.

**Live demo:** _add your GitHub Pages link here after enabling it (see Deployment below)_

## Features

- **Hero section** with an animated "digital rain" canvas background
- **About** section with a short bio
- **Skills** grid
- **Projects** section — each project card includes:
  - Project name
  - Description
  - Duration
  - Client feedback (optional, shown when available)
  - Screenshot / image
  - Link to the live app and/or source code
- **Certifications** section with certificate thumbnails and links to view the full image
- **Contact** section with a mailto link
- Fully responsive layout (mobile, tablet, desktop)
- Scroll-reveal animations via `IntersectionObserver`
- Respects `prefers-reduced-motion`

## Tech Stack

- **HTML5** — semantic markup
- **CSS3** — custom properties, CSS Grid/Flexbox, no framework
- **Vanilla JavaScript** — canvas animation + scroll reveal, no build tools or dependencies

This is intentionally a **static site**: no backend, no database. Any "CRUD" behavior on individual project pages (e.g. a to-do list demo) runs entirely client-side.

## Project Structure

```
├── index.html          # Main page (all sections)
├── assets/              # Images (photo, project screenshots, certificates)
│   ├── hero-portrait.png
│   ├── project-portfolio.png
│   ├── project-taskflow.png
│   ├── project-recipebox.png
│   ├── certificate-css.png
│   └── certificate-html.png
└── README.md
```

## Running Locally

No build step required. Either:

1. Double-click `index.html` to open it directly in a browser, **or**
2. Serve it locally:
   ```bash
   python3 -m http.server 8000
   ```
   then open `http://localhost:8000` in your browser.

## Deployment (GitHub Pages)

1. Push this repo to GitHub (public repository, `main` branch).
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`.
4. Save — your site will be published at `https://<your-username>.github.io/<repo-name>/`.

## Notes

- The images in `assets/` are placeholders generated for submission. Replace `hero-portrait.png` with an actual photo, and the `project-*.png` / `certificate-*.png` files with real screenshots before final grading if required.
- Update the "Live Site" / "Source Code" links in each project card in `index.html` once your actual demo/project links are ready.

## Author

**Francis** — BSIT C, 3rd Year
Software Engineering — Prelim Project
