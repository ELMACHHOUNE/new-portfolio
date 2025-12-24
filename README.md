# New Portfolio

A lightweight responsive portfolio website built with plain HTML, CSS and JavaScript.

## Overview

This repository contains a personal portfolio site showcasing skills, experience and projects. It is intentionally simple and dependency-free so it's easy to host on static hosting services such as GitHub Pages or any static web server.

Key features:

- Responsive layout
- JSON-driven skills and projects data (`skills.json`, `projects/projects.json`)
- Lightweight, plain HTML/CSS/JS — no build step required

## File structure

Top-level files and folders (important ones):

- `index.html` — main landing page
- `404.html` — custom 404 page
- `skills.json` — skills data used by the site
- `assets/` — images and CSS
  - `assets/css/style.css` — main stylesheet
  - `assets/css/404.css` — styles for 404 page
  - `assets/images/` — image assets used by the site
- `js/` — site JavaScript
  - `js/app.js`, `js/script.js` — site scripts
  - `js/particles.min.js` — optional visual effect lib
- `experience/` — experience section (self-contained page)
- `projects/` — projects page and `projects.json`

## Getting started (view locally)

You can preview the site by serving it from a simple static server. From the repository root (where `index.html` is), run one of the following in PowerShell:

```powershell
# If you have Python installed (works with Python 3):
python -m http.server 8000

# Or using npm without installing globally:
npx http-server . -p 8000
```

Then open http://localhost:8000 in your browser.

Note: No build step is required. Files are ready to be served as static assets.

## Customize the site

- Edit content in the HTML files to modify layout and text.
- Update `skills.json` and `projects/projects.json` to change the displayed skills and projects.
- Replace images in `assets/images/` (keep or update the image paths referenced in HTML/JSON).
- Tweak styles in `assets/css/style.css` for visual changes.

## Deployment

This site is suitable for GitHub Pages or any static host (Netlify, Vercel, Surge, S3 + CloudFront).

To deploy on GitHub Pages (user/organization page or repo page):

1. Push this repository to GitHub.
2. In the repository settings enable GitHub Pages and point it to the `main` branch (or `gh-pages` branch if you prefer).

Alternatively, use a static hosting service and point it at the repository root.

## Accessibility & performance

- Keep images optimized (use compressed JPEG/PNG/WebP) to improve performance.
- Ensure alt text is present on images for accessibility.
- The project is intentionally minimal to keep load times low.

## Contributing

This project is a personal portfolio template. If you'd like to suggest improvements, open an issue or submit a pull request. Small suggested additions:

- Add a `package.json` and development scripts if you want a build pipeline.
- Add simple unit or integration tests for any custom JS logic.

## License

You can choose an appropriate license for your portfolio. If unsure, consider the MIT License for permissive reuse. Add a `LICENSE` file if you want to make the license explicit.

## Contact

If you want help customizing this repository or deploying it, update this section with your preferred contact info (email, social handles, etc.).

---

Small and portable — perfect for hosting as a static personal portfolio.
