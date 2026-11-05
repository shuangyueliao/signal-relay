# Signal Relay

A free, original single-file HTML5 puzzle game. A disaster-region map shows
contour-line terrain: hills, valleys and dense forest. You have a limited
budget to place radio relay towers so that **every village receives the
signal**.

## How it plays

- **Line-of-sight coverage** — a tower's signal travels in a straight line and
  is blocked by hills, casting real *signal shadows* (visible as bites cut out
  of each tower's coverage circle).
- **Forest decay** — tree canopy weakens the signal: every forest cell on the
  path shortens the effective range (×0.6 attenuation).
- **Three tower classes** — Small (range 150, $30), Medium (220, $50),
  Large (300, $80).
- **Objective combos across 25 hand-made levels**: cover all villages, give
  marked villages *dual-tower redundancy* (≥2 towers each), stay inside the
  budget, and in network levels chain towers so neighbouring coverage circles
  overlap by at least 20% of the smaller circle.
- **Stars** are awarded by budget saved: ≥30% left = 3 stars, ≥15% = 2 stars.
  Best remaining budget per level is stored locally, so a level can be replayed
  to squeeze the budget further.

## Controls

- Mouse / touch: pick a tower size, tap the map to place, tap a tower to remove
  it (full refund).
- Keyboard: `1`/`2`/`3` select tower size, `M` mute, `Esc` back to levels.

## Tech

- Single `index.html`, zero external assets: all graphics are procedural
  canvas (contour bands, hatched highlands, tree canopies) and all audio is
  synthesized with WebAudio.
- Portal SDKs load only on their own domains (CrazyGames / GameDistribution
  domain guard) and never on standalone hosting.
- Vanilla JavaScript + Canvas + WebAudio. No frameworks, no tracking, no
  external links.
- Runs offline once loaded. ~44 KB.

## Run

Open `index.html` in any modern browser, or serve the folder:

```
python3 -m http.server 8080
```

## Play online

https://shuangyueliao.github.io/signal-relay/
