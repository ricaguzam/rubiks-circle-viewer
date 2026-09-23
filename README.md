# Rubik Circle Viewer

Local web app: set a 3×3 Rubik's cube state and see a 3D cube (left) synced with a concentric-circle sticker net (right).

## Run locally

```bash
cd rubiks-circle-viewer
npm start
```

Or without npm:

```bash
python -m http.server 8080
```

Open the printed URL (typically http://localhost:3000 or http://localhost:8080).

## Controls

- **Layer buttons** — apply Singmaster moves (`U`, `R'`, `F2`, …) with synced 3D spin + circle-dot slide
- **Scramble / Reset / Undo** — scramble animates quickly; reset/undo/load snap instantly
- **Moves** — paste a sequence like `R U R' U'` and click Apply (queued animations)
- **Facelets** — paste a 54-character string (`URFDLB` face order, 9 stickers each) and click Load

## Circular net

Three circle centers on an equilateral triangle, three concentric radii each.
Every crossing of circles from different centers is a sticker slot (54 total).
On a turn, dots slide along a shared circumference (lane), not through open space.
# rubiks-circle-viewer
