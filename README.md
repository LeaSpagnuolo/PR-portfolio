# CHERRY LINE — Carousel controls refinement

This package keeps the three-media carousel design and changes only video playback controls and navigation styling.

## Changes
- Removed the custom `ACTIVATE SOUND` / `OPEN VIDEO WITH SOUND` overlay buttons.
- Local videos use native browser controls, with sound enabled and no autoplay. Visitors can play, pause, seek, and adjust volume using the standard controls.
- YouTube embeds use their built-in controls and do not autoplay. Instagram embeds no longer have a custom overlay link on top of the media.
- Carousel navigation arrows use a motorsport-inspired dark-cherry treatment and sit outside the media area on desktop; on smaller screens they remain at the outer edges of the carousel.
- Preserves the three-media layout and natural media aspect ratios.

## Install
Replace `index.html`, `styles.css`, and `app.js` in the existing GitHub repository. Keep the existing `Media/` folder unchanged.

## Validation
`app.js` passes `node --check` and the ZIP archive passes `unzip -t`. Browser playback and final responsive layout should still be checked on the published GitHub Pages site.
