# CHERRY LINE — urgent media and Hero fix

Replace only `index.html`, `app.js`, and `styles.css` in the existing GitHub repository. Keep the existing `Media/` folder untouched.

Changes:
- Sport/School carousel adds only static files that actually exist in the published `Media/` folder, preventing missing paths from becoming broken slides.
- Sport Content 7 tries common exact-case filename variants for `.mov` and `.mp4`; the expected original `Media/Sportcontent7.mov` remains first.
- Media decoding errors now report a browser playback issue rather than falsely claiming the file is missing.
- A reload explicitly returns the page to the Hero/top position and clears a retained hash.

After publishing, hard-refresh with Cmd+Shift+R. If Sport Content 7 still does not appear, the filename or file itself in the repository differs from the candidates; confirm the exact spelling in GitHub.


## Final polish (30 October 2026)
- Desktop Hero fills exactly one viewport so the About section does not peek into view.
- Native fullscreen videos preserve their intrinsic aspect ratio, including portrait 9:16 videos.
- Sport Content and School Content descriptions remain on one line; long lines can be scrolled horizontally without truncating the text.
- Motorsport photo galleries advance automatically every 3.8 seconds, matching the About carousel timing. Manual arrows/dots reset the timer.


## Follow-up corrections (30 October 2026)
- Sport and School descriptions use natural wrapping: one line when they fit, a second line only when needed.
- Video side previews use captured frames instead of empty black panels; placeholder backgrounds are transparent.
- Carousel videos use a custom fullscreen control that fullscreen-expands the slide wrapper, preserving portrait 9:16 or landscape 16:9 orientation. Native fullscreen controls are disabled where supported.
- Project video embeds load eagerly so they are already present when the visitor scrolls to those sections.
- Spotify and YouTube preview embeds also load eagerly rather than waiting for the visitor to scroll close to them.\n
## Final finishing pass (30 October 2026)
- Let's Talk has an explicit full-bleed cherry background and no top border/seam.
- Sport Content and School Content descriptions wrap naturally at the available width on desktop and mobile; no horizontal clipping or line clamp.
- Video side thumbnails are generated from a decoded frame of the actual video, with a short seek to avoid blank opening frames.
- Motorsport galleries use a more distinctive angular cherry / motorsport visual treatment while retaining their existing controls and automatic rotation.
- Fullscreen on a content-carousel video opens the full frame and keeps the video's native aspect ratio.


## Final finishing pass (30 October 2026)
- Let's Talk fills the full laptop/desktop viewport in cherry burgundy and covers the seam above.
- Formula / Motorsport gallery photos now crossfade with a gentle scale/settle motion instead of a hard cut.
- Video side thumbnails are captured around 1.05 seconds, with a second attempt further into clips if the first chosen frame is nearly black.
- Instagram side cards use a dark cherry reel-style poster instead of the blank white unloaded embed; the actual Instagram player is loaded for the centered active slide.


## CHERRY LINE V5 — Hero spacing + personal soundtrack
- On desktop/laptop, the Hero portrait is shifted 5 mm to the right for more breathing room beside the surname.
- Added a closed-by-default right-edge soundtrack tab. Clicking it slides out a Spotify playlist drawer with the supplied playlist embed; it can be closed with the X, the tab, Escape, or by clicking outside.
- Drawer is responsive on mobile and respects reduced-motion preferences.
- No existing Media assets or portfolio sections were changed.
