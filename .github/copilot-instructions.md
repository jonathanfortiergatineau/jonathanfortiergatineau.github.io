# Copilot Instructions for AI Agents

## Project Overview
This repository is a personal portfolio and project showcase site, primarily static, built using HTML, CSS (Bootstrap-based), and JavaScript. It is deployed via GitHub Pages using a Jekyll workflow, but most content is static and not Jekyll-specific.

## Key Structure
- `/assets/`: Main CSS (`css/style.css`), JavaScript (`js/main.js`), images, and SCSS (not actively used).
- `/projects/`: Custom project pages, including interactive demos (e.g., `experimental/mouse_trail.html`, `pianopractice/index.html`).
- `/old site/`: Legacy site files for reference or migration; not actively maintained.
- `.github/workflows/jekyll-gh-pages.yml`: GitHub Actions workflow for deployment.

## Patterns & Conventions
- **Templates**: Main site uses BootstrapMade templates (see comments in HTML/CSS/JS for template details and licensing).
- **No build step**: All files are edited directly; there is no bundler, transpiler, or package manager.
- **Static assets**: Reference assets with relative paths (e.g., `assets/css/style.css`).
- **Custom JS**: Place new scripts in `assets/js/` and link them in HTML as needed.
- **Legacy code**: Files in `old site/` are for reference only—do not update unless migrating content.

## Developer Workflows
- **Deploy**: Push to `main` branch triggers GitHub Actions to build (with Jekyll) and deploy to GitHub Pages.
- **No tests/builds**: There are no automated tests or build scripts. Manual browser testing is expected.
- **Debugging**: Use browser dev tools; no source maps or advanced debugging setup.

## Integration Points
- **External dependencies**: Bootstrap, FontAwesome, and other vendor CSS/JS are loaded via CDN in HTML files.
- **No backend**: All content is static; no server-side code or API integration.

## Examples
- To add a new project: create a new HTML file in `/projects/` and link assets relatively.
- To update site styles: edit `/assets/css/style.css` directly.
- To deploy: commit and push to `main`—deployment is automatic.

## Special Notes
- Preserve template attributions and licenses in all distributed files.
- Do not introduce build tools or frameworks unless explicitly requested.
- When migrating content from `old site/`, update asset paths and modernize code to match current structure.

---
For questions or unclear conventions, ask for clarification or check template comments in the main HTML/CSS/JS files.
