# CK42X Hermetic Tarot Trainer

A public, static Hermetic Tarot study trainer for learning the structure behind the cards before reading them intuitively. It covers the Tree of Life, Hebrew letters, zodiac decans, court cards, daily draws, a curriculum journey, quizzes, a local journal, and a personal study lab.

This is a public-safe release of a CK42X private study prototype. It runs entirely in the browser and stores personal progress only in the user's local browser storage.

## Features

- 148-lesson structured curriculum
- Tree of Life and 22-path reference view
- 36-decan zodiac wheel
- All 78 card correspondence cheat sheet
- Random and systematic draw modes
- Local-only journal and study notes
- Local-only progress, quiz, and draw tracking

## Run locally

No build step is required. Serve the directory with any static file server:

```bash
python3 -m http.server 4173
```

Then open `http://localhost:4173`.

Opening `index.html` directly from disk may work in some browsers, but a local static server is recommended because the app loads `data/tarot-data.json`.

## Data and privacy

The trainer ships with static correspondence and curriculum data in `data/tarot-data.json`. User progress, draws, quiz attempts, journal entries, and study-lab notes stay in `localStorage` under the `ck42x.hermeticTarot.v1` key. Nothing is sent to CK42X or any server.

No external services are required at runtime. The app is designed for static hosts such as GitHub Pages.

To reset local progress, clear site data for the app in your browser.

## Licensing and attribution notes

- Code is released under the MIT License.
- Tarot, Qabalistic, astrological, and Golden Dawn-style correspondences are presented as study/reference material.
- This repository does not include proprietary card images.
- Deck-specific names or references are for identification and study context only; verify rights before adding scanned or commercial card artwork.
