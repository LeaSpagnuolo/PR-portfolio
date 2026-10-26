# CHERRY LINE — W2W & Content carousel correction

This patch updates the existing static site files only. Keep your existing `Media/` folder (uppercase M) and all of its contents unchanged.

## Included fixes
- Women2Women uses the supplied YouTube video ID `Qc660Zu_hZI` in a landscape 16:9 embed rather than relying on the local `Media/W2W.mp4` playback.
- Sport Content 1 and 3 are substituted in their original carousel slots instead of being appended a second time.
- School Content no longer receives an extra appended hosted vlog on top of the local media list.
- Content slides use the loaded media's native width/height ratio, `object-fit: contain`, and a thin outline that sits just outside the media instead of cropping it.
- Video fullscreen keeps the media contained within the screen while preserving its native proportions.

## Install
1. Unzip this archive.
2. Replace `app.js`, `index.html`, and `styles.css` in your existing GitHub repository.
3. Do not replace, rename, or upload over your existing `Media/` folder.
4. Commit and wait for GitHub Pages to redeploy.

## Validation
`app.js` passes `node --check`, and the ZIP archive passes integrity testing. External YouTube/Instagram playback still depends on the platform's embed permissions and the published site/browser; it cannot be fully verified offline.
