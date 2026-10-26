# CHERRY LINE — Carousel polish update

This update is based on the existing CHERRY LINE code. It keeps the `Media/` directory name with its uppercase M and does not include or rename any media files.

## Included changes
- Removes visible arrow and dot navigation from About, Sport Content, School Content, Spa and 24H carousels.
- Enables swipe/drag navigation for carousels and adds seamless edge clones for Sport/School and About so wrapping does not visibly animate backwards.
- Keeps each Sport/School media item at its own intrinsic ratio; portrait videos stay portrait in their frame.
- Starts local video previews muted and looping so the user can see moving frames instead of a black idle frame where browser playback permits it.
- Adds muted autoplay/loop parameters to YouTube preview embeds. Browser policies and provider restrictions may still block autoplay or Instagram embeds.

## Install
Replace `app.js`, `index.html`, and `styles.css` in the existing repository. Keep the existing `Media/` folder and all media filenames unchanged. Commit and wait for GitHub Pages to deploy.

## Validation
The JavaScript syntax and ZIP integrity are checked. This package has not been visually tested on the published website; external video playback still depends on YouTube/Instagram permissions and browser autoplay policy.
