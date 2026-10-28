# CHERRY LINE — Media Carousel & Ratio Fix

This package restores the three-card Sport Content / School Content carousel (previous, active, next) and preserves each media's natural dimensions.

## Replace these files
- `index.html`
- `styles.css`
- `app.js`

Keep your existing `Media/` folder unchanged in the root of the GitHub repository. The carousel references it with case-sensitive paths.

## Changes
- Restores the three-media composition instead of a horizontal strip of 4–5 cards.
- Fits each image/video using its natural aspect ratio (`object-fit: contain`) so 16:9 videos are not forced into a 9:16 frame.
- Includes `Media/Sportcontent7.mov` in the Sport Content carousel.
- Adds `Media/Schoolcontent4.png` (the poster) to School Content.
- Includes hosted social videos as additional carousel items instead of replacing local media slots.
- Keeps the visible previous/next buttons and clickable side previews.

After upload, wait for GitHub Pages to deploy and hard-refresh the site (`Cmd + Shift + R`). JavaScript syntax was checked; the live site and exact deployed filenames have not been independently browser-tested.
