# Rosa Ramalho — Galeria AR

Marker-based augmented reality demo. One page per 3D model, plus a menu.

## Files (all must stay in the repo root)
- `index.html` — menu (start here)
- `devil.html`, `musician.html`, `monkey.html`, `fish.html` — one AR page per model
- `devil.glb`, `musician.glb`, `monkey.glb` — stylised *figurado* pieces (animated)
- `fish.glb` — realistic fish model with textures (animated swim)
- `rosa-fish.patt`, `marker_rosa_fish.png` — the OPTIONAL custom marker (see below)

## The marker
By default every page uses the standard **Hiro** marker, which tracks far more
reliably than a custom one. Print the official Hiro marker from:
https://ar-js-org.github.io/AR.js-Docs/marker-based/  (the "Hiro" image)
Print it on matte paper (~10-15 cm), keep it flat and well lit.

### To use the custom fish marker instead
In any page, find these two lines near `<a-scene>`:
    <!-- <a-marker type="pattern" url="rosa-fish.patt"> -->
    <a-marker preset="hiro">
Swap them: uncomment the first, delete the `preset="hiro"` line. Then print
`marker_rosa_fish.png`.

## Use
Open the GitHub Pages URL on a phone (Android Chrome / iPhone Safari), allow the
camera, tap a model, point at the printed marker.

## Troubleshooting
- Nothing appears: you're not pointing at the *printed* marker, or lighting is poor.
- Updated a file but see the old one: hard refresh / open in a private tab (cache).
