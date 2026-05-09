# AGENTS.md

## Repo Shape
- This repo is a plain static GitHub Pages site. There is no package manager, build step, test runner, or CI config.
- Main pages live at the repo root: `index.html`, `stories.html`, and `contact.html`.
- Shared styling is all in `style.css`.
- `.nojekyll` is intentional for GitHub Pages. Keep it unless the hosting setup changes.

## Editing Rules
- Keep links and asset references relative, not root-based. Current pages use `./index.html`, `./stories.html`, `./contact.html`, and `./style.css` so the site works at the GitHub Pages project URL.
- If you add assets, reference them with relative paths from the HTML files for the same reason.
- There is no templating or component system here; repeated header/footer markup must be updated in each HTML page.

## Content/UX Constraints
- The current design direction is intentionally plain and editorial, not heavily decorative.
- The homepage order is deliberate: hero/title, `About the page`, `Meet the storyteller`, then `Highlight categories`.
- The site currently uses abstract artwork blocks instead of a real owner photo. Do not reintroduce a photo dependency unless the user provides an actual file.

## Contact Form
- `contact.html` uses a Formspree placeholder endpoint: `https://formspree.io/f/your-form-id`.
- Replace only the form endpoint when wiring the form for production; the site has no backend mail handling.

## Verification
- There is no repo-local build or test command. Verify changes by opening the HTML pages directly in a browser and checking desktop/mobile layout.
- After navigation edits, click through all three pages to confirm active nav links and relative paths still work.
