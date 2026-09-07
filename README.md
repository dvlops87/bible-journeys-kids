# The Shepherd King

A bilingual (English/Korean) interactive retelling of David and Goliath (1 Samuel 16–18), built as a single-file HTML/CSS/JS game — no build step, no dependencies.

- **[index.html](index.html)** — the game itself. Open directly in a browser, or serve via GitHub Pages.
- **[report.html](report.html)** — a project report covering the narrative design, duel physics, quality review, and development iteration log.

## Highlights

- Seven narrative chapters dramatizing nine cited passages from 1 Samuel 16–18
- A physics-based slingshot duel (drag-to-aim or keyboard: arrow keys + Enter/Space) whose launch speed is solved from the live canvas geometry, so it reaches Goliath at any screen size
- Three branching "parallel timeline" detours for choices Scripture doesn't take, clearly marked as non-canon
- Full English/Korean localization with an in-game language toggle
- `prefers-reduced-motion` support, keyboard operability, and `localStorage`-backed best-score/language persistence

## Running locally

No build step — just open `index.html` in a browser, or serve the folder with any static file server, e.g.:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.
