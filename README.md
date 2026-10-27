CHERRY LINE — CONTENT CAROUSEL + ABOUT DESKTOP FIX

Included files:
- index.html
- styles.css
- app.js

Install into the existing GitHub Pages repository by replacing these three files only.
Keep the existing Media/ folder exactly as it is (capital M). Do not create a new repository.

Changes:
- Sport Content and School Content show up to three cards: active center + one preview on each side.
- Center card dimensions adapt to the media's actual ratio; side cards remain previews and do not play.
- YouTube slides use thumbnail previews while inactive; the embed is loaded only for the active slide.
- The ACTIVATE SOUND control remains the explicit user action for sound.
- Local video playback is paused and muted when the carousel leaves the viewport or the browser tab becomes hidden.
- About carousel auto-advances every 3.8 seconds on desktop and mobile, with larger visible clickable dots beneath the image.
- Global page canvas stays dark outside section backgrounds to avoid white gaps around the page.

Validation performed: JavaScript syntax checked with Node.js; ZIP integrity checked.
Not performed: full live browser test against GitHub Pages. YouTube/Instagram embeds and autoplay can still be affected by browser/provider restrictions.
