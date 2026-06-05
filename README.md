# Tic-Tac-Toe — Z vs 3

A browser-based tic-tac-toe game with a neon synthwave theme and a 3D board.
Built as a single, self-contained HTML file — no installation, no dependencies,
no build step. Just open it and play.

**Play:** open [`Test_Project/index.html`](Test_Project/index.html) in any modern browser
(double-click the file, or drag it into a browser window).

## How to Play

- **You are `Z`** (electric cyan). **The computer is `3`** (hot magenta).
- These replace the traditional X and O marks.
- You always move first. Click any empty tile to place your `Z`; the computer responds automatically.
- Get three of your marks in a row — horizontally, vertically, or diagonally — to win.
  The winning line lights up in acid lime and pulses.
- If all nine tiles fill with no winner, it's a draw.

## Features

- **Player vs Computer** — the computer uses a simple priority-based strategy:
  1. Take a winning move if one is available.
  2. Block your winning move if you're about to win.
  3. Take the center if it's open.
  4. Otherwise, play a random open tile.
- **Scoreboard** — tracks wins for You, the Computer, and Draws across games in the current session.
- **New Game** — clears the board for a fresh round while keeping the running score.
- **Reset Scores** — sets all three counters back to zero.
- **3D neon board** — the board is tilted in 3D space; tiles are raised blocks that
  pop up on hover and press down when clicked, all in a synthwave color palette.

> Note: scores are kept for the current browser session and reset when the page is reloaded.

## Tech

- Plain HTML, CSS, and vanilla JavaScript in one file (`Test_Project/index.html`).
- No frameworks, no libraries, no build tooling.
- 3D effect via CSS `perspective` / `transform`; neon look via gradients and `text-shadow` glows.

## Revision History

| Version | Date       | Changes                                                                 |
|---------|------------|-------------------------------------------------------------------------|
| 1.0     | 2026-06-05 | Initial release: browser-based tic-tac-toe, player (`Z`) vs computer (`3`), New Game button, win/draw detection. |
| 1.1     | 2026-06-05 | Added a scoreboard tracking You / Draws / CPU, plus a Reset Scores button. |
| 1.2     | 2026-06-05 | Restyled with a 3D tilted board and a wild neon synthwave color scheme (glowing marks, raised tiles, pulsing win highlight). |
