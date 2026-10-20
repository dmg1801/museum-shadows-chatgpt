# Museum of Shadows

A playable, no-build Phaser 3 archaeological horror platformer. Four halls, twelve relic fragments, sanity, ghosts, checkpoints, procedural art and synthesized audio, pyramid finale and twist ending.

## Play
Open `index.html` in a browser with internet access (Phaser 3 loads from a CDN). For local development, a static server such as `python -m http.server 8000` is optional. Audio begins after your first interaction, as required by browsers.

## Controls
Desktop: A/D or arrows to move; Shift to run; Space/W/Up to jump; E/Enter to interact; F for flashlight; R to restart after ending.

Mobile: virtual left joystick, JUMP, ACT, LIGHT and RUN. Landscape recommended.

## Objective
Collect three glowing fragments per hall. Approach the far-right door and press ACT/E. Plaques near the beginning of each hall restore sanity. Candles and flashlight slow darkness-related sanity loss. Ghosts drain sanity. Checkpoints update as you advance.

## GitHub Pages
1. Create a public GitHub repository.
2. Upload the **contents** of this folder to the repository root (so `index.html` is at the root).
3. In Settings → Pages → Build and deployment, choose **Deploy from a branch**, `main`, `/ (root)`, and Save.
4. Wait for GitHub to publish the Pages URL.

## Project
- `index.html`: page and touch UI
- `css/style.css`: responsive full-screen layout
- `js/game.js`: Phaser scenes, procedural placeholder sprites, gameplay and synthesized sounds
- `assets/`: reserved for future original pixel art and sound assets

## Notes / scope
This is a complete playable **prototype**, not a fully produced commercial game. Art is procedurally drawn placeholder art; ambient audio and action sounds are synthesized rather than supplied as recorded WAV files. Phaser is fetched from a pinned CDN version, so the first launch requires internet. For fully offline hosting, download Phaser 3.90.0 locally and change the script reference. No npm/build process required. Original third-party artwork or recordings are not included.


## v1.2 fixes
- Restored the original illustrated ghost/candle/statue atmosphere from the first corrected version.
- Improved jump impulse and platform heights.
- Prevented a crash at the Egyptian exit: the pyramid cinematic no longer updates a destroyed physics body.
- Reset camera bounds for the playable epilogue.
- Flashlight light is cleared between scenes.
