# Two Journeys

A bilingual (English/Korean) interactive retelling of two callings from Scripture — David (1 Samuel 16–18) and Moses (Exodus 2–14) — built as a single-file HTML/CSS/JS game. No build step, no dependencies. Written simply for young readers (grades 1–6).

## Play it live

- 🎮 **[Play the game](https://tinyurl.com/bible-journeys-kids)**
- 📄 **[Read the project report](https://dvlops87.github.io/bible-journeys-kids/report.html)**

Or browse the source:

- **[index.html](index.html)** — the game itself. Open directly in a browser, or serve via GitHub Pages.
- **[report.html](report.html)** — a project report covering the original narrative design, duel physics, and quality review (written before the Moses track was added).

## Highlights

- A character-select screen: play David's rise from shepherd to king, or Moses' call from fugitive shepherd to deliverer
- Every scene reads first and confirms second — picking an option only marks it selected; nothing is recorded or advanced until you press **Next**, so there's no accidental click-through
- Two physics-driven minigames:
  - **The Duel** (David) — drag-to-aim or keyboard slingshot; launch speed is solved from the live canvas geometry so a good throw reaches Goliath at any screen size
  - **The Waters Stand Apart** (Moses) — press-and-hold (pointer or Space/Enter) to keep the Red Sea parted while Israel crosses; let go too long and the walls start to close
- Seven branching "parallel timeline" detours (3 for David, 4 for Moses) for the choices Scripture doesn't take, clearly marked as non-canon and always returning you to the fork rather than ending the game
- Full English/Korean localization with an in-game language toggle that never mixes languages mid-journey
- `prefers-reduced-motion` support, full keyboard operability, and `localStorage`-backed best-score/language persistence per story

## Running locally

No build step — just open `index.html` in a browser, or serve the folder with any static file server, e.g.:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.
