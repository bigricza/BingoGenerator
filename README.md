# BINGO — Social Club Caller & Card Printer

A fully self-contained bingo game designed to run on a large screen at a social club. No server, no dependencies, no build step — just open `index.html` in a browser and play.

## Features

- **Two game types** — 75-ball (American) and 90-ball (UK)
- **Animated tumbler** — spinning ball cage with procedural audio (Web Audio API, no sound files)
- **Traditional call phrases** — "Two Little Ducks", "Two Fat Ladies", all 90 of them
- **Full number board** — color-coded, highlights called numbers with animations
- **Last 10 tracker** — mini-ball strip showing recent calls
- **Game persistence** — state saved to localStorage; refresh won't lose your game
- **Card printer** — generate 1–60 random cards and print them on A4 paper
- **Keyboard support** — press Space to spin
- **Responsive** — works on desktop (two-panel) and mobile (stacked)

## Quick Start

1. Open `index.html` in any modern browser
2. Choose 75-ball or 90-ball
3. Click **SPIN** (or press Space) to call numbers
4. Display on a projector or large TV for the club

## Printing Cards

1. Click **Print Cards** in the header (or open `cards.html` directly)
2. Select game type and number of cards (up to 60)
3. Click **Generate**, then **Print**
   - 75-ball: 2 cards per A4 page
   - 90-ball: 4 cards per A4 page

## Files

| File | Purpose |
|------|---------|
| `index.html` | Game caller — spin, display, board |
| `cards.html` | Card generator and print layout |

That's it. Two files, ~43 KB total, zero dependencies.

## Tech

- Vanilla HTML / CSS / JavaScript
- CSS Grid + Flexbox for layout
- CSS custom properties and keyframe animations
- Web Audio API for procedural tumbler rattle and reveal chime
- LocalStorage for game state persistence

## Browser Requirements

Any modern browser (Chrome, Edge, Firefox, Safari). Requires CSS Grid, ES6+, and Web Audio API support.
