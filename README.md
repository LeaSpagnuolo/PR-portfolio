# CHERRY LINE — About + Content carousel correction

This patch is based on the latest available CHERRY LINE code and preserves the `Media/` directory name with uppercase `M`. It does not include, rename, or delete any media files.

## Fixes in this patch
- Restores About carousel movement by sizing its track/slides in pixels and translating by the viewport width, including after resizing.
- Keeps Sport Content and School Content media at the source's intrinsic aspect ratio; the surrounding frame adds a small outline without cropping or forcing the media into 9:16.
- Removes clipping caused by a fixed stage height that was shorter than the media frames. Portrait videos remain portrait; landscape media remains landscape.
- Keeps arrows and dot navigation hidden, preserving swipe/scroll interaction.

## Install
Replace `app.js`, `index.html`, and `styles.css` in the existing repository. Keep the existing `Media/` folder and all media filenames unchanged. Commit and wait for GitHub Pages to deploy.

## Validation and limitation
JavaScript syntax and ZIP integrity are checked. The published website was not available for a full browser-based visual/playback test. Actual video playback can still depend on the media codec, hosting path, and external provider restrictions.
