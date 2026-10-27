# CHERRY LINE — Content Carousel Playback Fix

This patch updates the existing `app.js`, `index.html`, and `styles.css` only. Keep your existing `Media/` folder unchanged (capital M).

## Changes
- Content carousels display the active media in the center, with at most one distinct neighboring media on each side.
- Duplicate loop clones are removed; navigation wraps the index instead of duplicating slides in the DOM.
- Only the centered local video is played. Neighboring videos are paused and can show a decoded preview frame.
- Embedded video iframes are loaded only when centered and unloaded when moved to the sides, preventing multiple videos from playing at once.
- Media dimensions are derived from each image/video's intrinsic ratio; `object-fit: contain` avoids cropping and keeps portrait video portrait.
- Sport and School carousels use swipe navigation; arrows and dots remain hidden.
- All static media references retain the exact `Media/` capitalization.

## Install
1. Extract the ZIP.
2. Replace `app.js`, `index.html`, and `styles.css` in your existing GitHub repository.
3. Do not replace or rename the `Media/` folder.
4. Commit and wait for GitHub Pages to deploy.

Validation performed: JavaScript syntax (`node --check`) and ZIP integrity. Browser playback on the published site was not available for live verification. Browser autoplay restrictions and third-party embed permissions can still affect external players.
