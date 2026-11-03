# Sokoban Push — Store Submission Materials

## Short description (CrazyGames / GameDistribution / itch.io, <=200 chars)

Classic sokoban: push every wooden crate onto its glowing target. One push at
a time, no pulling — think before you shove. 12 machine-verified levels, star
ratings, unlimited undo.

(180 chars — verified, under the 200 limit)

## Details

- Genre: Puzzle / Casual / Sokoban
- Controls: Arrow keys / WASD on desktop; on-screen D-pad and swipe gestures on
  mobile. U = undo (unlimited), R = restart, M = mute.
- Features: 12 handcrafted levels (teaching pushes -> order-planning depots),
  star ratings (3 stars at or under par, 2 within 1.5x par), per-level best
  scores and level unlocking saved in localStorage, moves & pushes counters,
  unlimited undo via full state history, level-select map screen.
- Rules: the worker moves one tile per step; walking into a crate pushes it one
  tile if the space beyond is free; pushes into walls or other crates are
  rejected; a crate can never be pulled. All crates on glowing targets = level
  clear.
- Visuals: warehouse theme drawn fully in canvas — brick walls, concrete floor
  tiles, wooden crates with forklift fork-slot imprints, pulsing glowing goal
  markers, push-squeeze crate animation, bumper feedback on rejected moves.
- Audio: procedural WebAudio synthesis (footstep, crate push, crate-locked
  chime, victory arpeggio, reject thud), mute toggle persisted.
- Tech: Vanilla JavaScript, Canvas, WebAudio. Single-file HTML5 (no external
  assets, no CDN, no fonts, no tracking), works offline once loaded. Every
  level verified solvable by a BFS solver; par values derived from solver
  optima (par = optimal + 25%).

## Tags

sokoban, puzzle, boxes, warehouse, casual, logic, brain, single-file, mobile-friendly

## CrazyGames submission checklist
- [x] Self-contained index.html (SDK loads only on crazygames domains)
- [x] gameplayStart / gameplayStop / happytime wired (plus loadingStart / loadingStop in loader)
- [x] Responsive (canvas scales to viewport, portrait & landscape, touch D-pad)
- [x] No external links inside gameplay, no analytics
- [ ] Cover: cover-16x9.png (1280x720) — to be captured
- [ ] Screenshots: screenshot-raw.png (1280x800) — to be captured

## GameDistribution
- Upload: sokoban-push-gd.zip (contains index.html only)

## itch.io
- Upload: sokoban-push-itch.zip, mark "This file is playable in browser",
  entry file: index.html, viewport embed: fits any size (board scales), kind: html
- Pricing: $0 (donations optional)
