# Jane Street Puzzle Practice

Smaller, playable versions of [Jane Street's monthly puzzles](https://www.janestreet.com/puzzles/). Warm up on little boards until the rules click, then take on the real one.

**Play:** https://jimmyli2468.github.io/jane-street-puzzle-practice/

Works on iPhone, iPad, Android and desktop browsers. Each page is one self-contained HTML file with no build step. Progress is saved in the browser's local storage.

## Puzzles

| Month | Puzzle | What you get |
| --- | --- | --- |
| October 2026 | [It's a Metric, Too](https://jimmyli2468.github.io/jane-street-puzzle-practice/its-a-metric-too/) | 48 practice boards (4×4 to 7×7), each with exactly one solution, plus the original 11×11 with a rule checker. [Capitol magnets](https://jimmyli2468.github.io/jane-street-puzzle-practice/its-a-metric-too/magnets.html) treats clues as magnets that push capitols away up close and pull them back from afar, pops the ones squeezed too hard, and maps where the rest come to rest. |

## Why a website instead of the HTML file

If you send an `.html` file to an iPhone or iPad (through iMessage, AirDrop, email or Files), iOS opens it in Quick Look, and Quick Look does not run JavaScript. The page shows up blank. The same file served from a URL runs normally in Safari, which is why these pages are hosted on GitHub Pages.

## Adding a puzzle

1. Create a folder named after the puzzle, such as `my-next-puzzle/`, with an `index.html` inside. Keep everything (CSS, JS, data) in that one file.
2. Add a `← All puzzles` link pointing to `../`.
3. Add a card for it at the top of the list in the root `index.html`, and a row at the top of the table above.
4. Commit and push to `main`. GitHub Pages redeploys in about a minute.

To preview locally:

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Disclaimer

This is an unofficial fan project and is not affiliated with Jane Street. The puzzles, their rules and the original grids belong to Jane Street. This repository only contains practice versions and checkers, not answers to open puzzles.
