# CF-JEPA project website

A single-page research site for **CF-JEPA: Improving Robustness of JEPA World Models via
Controllability Factorization** (ICRA 2027 submission).

## Files
- `index.html` — the page (self-contained; MathJax loaded from CDN for the equations).
- `styles.css` — styling.
- `assets/fig/` — figures rendered from the paper PDFs (method overview, tasks, result curves, reconstructions).
- `assets/media/` — rollout GIFs and the overview video.
- `assets/paper/CF-JEPA.pdf` — the paper.

## Preview locally
Open `index.html` directly, or serve the folder (recommended so the video/paths load cleanly):

```bash
cd website
python -m http.server 8000
# then visit http://localhost:8000
```

## Deploy to GitHub Pages
Push the repo and either:
- set Pages to serve from `/website` on the `main` branch, **or**
- move the contents of `website/` to the repo root (or a `docs/` folder) and point Pages there.

`.nojekyll` is included so the `assets/` folders are served as-is.

## Updating for camera-ready
The page is anonymized for double-blind review. When de-anonymizing, edit the
`.authors`, `.affil`, and BibTeX blocks in `index.html`, and drop the `.anon-note`.
