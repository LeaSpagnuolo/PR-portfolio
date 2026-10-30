# CHERRY LINE — urgent media and Hero fix

Replace only `index.html`, `app.js`, and `styles.css` in the existing GitHub repository. Keep the existing `Media/` folder untouched.

Changes:
- Sport/School carousel adds only static files that actually exist in the published `Media/` folder, preventing missing paths from becoming broken slides.
- Sport Content 7 tries common exact-case filename variants for `.mov` and `.mp4`; the expected original `Media/Sportcontent7.mov` remains first.
- Media decoding errors now report a browser playback issue rather than falsely claiming the file is missing.
- A reload explicitly returns the page to the Hero/top position and clears a retained hash.

After publishing, hard-refresh with Cmd+Shift+R. If Sport Content 7 still does not appear, the filename or file itself in the repository differs from the candidates; confirm the exact spelling in GitHub.
