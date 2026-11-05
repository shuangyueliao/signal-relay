# Signal Relay — Store Submission Materials

## Short description (CrazyGames / GameDistribution / itch.io)

Disaster struck the valley. Place radio relay towers on a contour-line
terrain map — hills cast signal shadows, forests weaken the signal — and
bring every village back on the air before the budget runs out.

(197 characters)

## Details

- Genre: Puzzle / Strategy / Casual
- Controls: Mouse / Touch (pick a tower size, tap to place, tap a tower to
  remove). Keyboard: 1/2/3 tower size, M mute, Esc level menu.
- Features:
  - Line-of-sight radio coverage: hills block the signal and cast real
    signal shadows on the map
  - Forest canopy attenuates the signal — effective range shrinks to 60%
  - 3 tower classes: Small (150 / $30), Medium (220 / $50), Large (300 / $80)
  - 25 hand-designed levels with growing objectives: full coverage, dual-tower
    redundancy for lifeline villages, budget limits, and relay-networking
    (neighbouring coverage circles must overlap by 20%)
  - Star rating by budget saved (3 stars at 30% remaining), per-level best
    saved locally — replay levels to squeeze the budget
  - Procedural contour-line maps, breathing coverage circles, tripod build-up
    animation, radio-static and confirmation sounds
- Tech: Vanilla JavaScript, Canvas, WebAudio. Single-file HTML5, no external
  assets, no tracking, no external links, works offline once loaded.
- Portal SDK: loads only on CrazyGames / GameDistribution domains
  (domain-guarded); gameplayStart / gameplayStop / happytime wired.

## Tags

puzzle, strategy, simulation, radio, towers, coverage, terrain, logic,
single-file, original

## CrazyGames submission checklist
- [x] Self-contained index.html (SDK loads only on portal domains)
- [x] gameplayStart / gameplayStop / loadingStart / loadingStop / happytime events wired
- [x] Responsive (canvas scales to fit, portrait-friendly, touch + desktop input)
- [x] No external links inside gameplay, no analytics
- [ ] Cover: cover-16x9.png (1280x720)
- [ ] Screenshots: screenshot-raw.png (1280x800)

## GameDistribution
- Upload package: signal-relay-gd.zip (contains only index.html)
- Genre: Puzzle / Logic

## itch.io
- Upload zip: signal-relay-itch.zip, mark "This file is playable in browser",
  entry file: index.html, viewport 480x600 (auto-fit), kind: html
- Pricing: $0 (donations optional)
