HOME VIEW V29 — LOTTIE LOADING + STEP-AHEAD PRELOADING

Replace:
- index.html
- styles.css
- app.js

NEW LOADING ANIMATION
Whenever navigation has to WAIT for a file, the presentation now shows:
Lottie/loading intro.json

The loader is a full-screen overlay and disappears automatically as soon
as the required asset is ready.

NOTE:
This version loads lottie-web from:
https://cdnjs.cloudflare.com/ajax/libs/lottie-web/5.12.2/lottie.min.js

STEP-AHEAD PRELOADING
The presentation now deliberately preloads the NEXT asset while the user
is viewing the current step.

Examples:
- Opening page -> preloads Blue Background + Title 01
- Title 01 -> preloads Plan assets
- Sphere -> preloads Blue Background + Title 02
- Title 02 -> preloads Vid_01
- Vid_01 -> preloads Vid_02
- Vid_02 -> preloads Vid_03
- Vid_03 -> preloads Vid_04
- Vid_04 -> preloads Vid_05
- Vid_05 -> preloads old method.mp4
- Old Method -> preloads new method.mp4
- New Method -> preloads stage.jpg
- Ownership -> preloads graph assets
- Graph -> preloads final Title 02 + Blue Background

If the next asset is already ready, the loader never flashes on screen.
It only appears when there is an actual wait.

REQUIRED EXISTING ASSET
Lottie/loading intro.json
