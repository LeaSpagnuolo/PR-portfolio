# CHERRY LINE — Carousel polish update

This update uses the existing static `Media/` folder (capital M). It does not include or rename your media files.

## Changes
- Sport Content and School Content show at most three distinct media: one centered active item and one smaller preview on each side.
- Only the centered video/embedded player is activated. Side videos are paused and external embeds are unloaded when they move off-center.
- Media dimensions follow each source's native ratio; portrait videos remain portrait, landscape videos remain landscape, with no forced 16:9 crop.
- The active center video attempts to play with sound. Browsers can block sound-on autoplay; if that happens, the center video remains available for a click/tap.
- About displays all four photo slots as a carousel, rotates automatically, and has clickable dots underneath.
- Motorsport galleries no longer advance automatically; users can take as long as they want and navigate with the existing controls, dots, or swipe. Inactive videos are paused.
- The existing `Media/` capitalization and the rest of the site files are preserved.

## Install
1. Extract the ZIP.
2. Replace `app.js`, `index.html`, and `styles.css` in the existing GitHub repository.
3. Leave the `Media/` folder untouched.
4. Commit and wait for GitHub Pages to deploy.

## Validation
JavaScript syntax and ZIP integrity are checked. The published site was not available for browser-level visual testing in this session. Sound-on autoplay is controlled by browser policy and may require a click/tap on the first video.
