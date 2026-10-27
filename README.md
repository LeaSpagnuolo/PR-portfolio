# CHERRY LINE — Content audio control fix

This patch is based on the latest available CHERRY LINE bundle. It preserves the `Media/` folder name with a capital M and does not include, rename, or replace media files.

## Sport Content and School Content
- The carousel shows no more than three cards: one central active item, one preview on the left, and one preview on the right.
- Local videos in the center start muted. Use **ACTIVATE SOUND** to restart that video from 00:00 with sound. The sound button is hidden on side previews.
- When a local video leaves the center, it is paused, muted, and reset to the beginning.
- YouTube embeds start muted in the center. **ACTIVATE SOUND** reloads the active video from the beginning with sound enabled. When the item leaves the center, its iframe is unloaded to stop playback/audio.
- Instagram Reels use an external link because Instagram does not reliably support controlled autoplay/mute behavior inside a third-party carousel.
- Media frames use the actual source ratio (portrait remains portrait, landscape remains landscape) rather than forcing everything to 16:9.

## About
- Four photos remain in the carousel with automatic rotation every 4.5 seconds.
- Dots underneath let the visitor select a photo directly; hovering/focusing pauses automatic rotation.

## Install
1. Extract the ZIP.
2. Replace `app.js`, `index.html`, and `styles.css` in the existing GitHub repository.
3. Keep the `Media/` folder intact.
4. Commit and wait for GitHub Pages to deploy.

## Validation and limits
JavaScript syntax (`node --check`) and ZIP integrity were checked. The live site was not tested in a browser in this session. Browser policies can block autoplay; if that happens, use the visible sound/play control. Embedded YouTube and Instagram behavior can also depend on provider settings.
