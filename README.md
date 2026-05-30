# AbbeyNB Launch Site

Static public launch build for AbbeyNB, a curated Catholic retreat and sacred-stay directory.

## Current launch safety notes
- Christ in the Desert Monastery is intentionally excluded after declining inclusion and photo use.
- Franciscan Renewal Center is held out of public launch until listing/photo permission is clarified.
- Christian Renewal Center, Abbey of Gethsemani, and New Camaldoli Hermitage have approved website-photo use for AbbeyNB; approved photos are stored locally under `assets/listings/`.

## Launch audit — 2026-05-29
- Repo/source verified: `/home/sandreu/abbeynb-live-site`, remote `sandreu-ai/AbbeyNB`, HEAD `f8b69ab` (`Add approved listing photos`).
- Safe local checks passed: `site-listings.json` parses as JSON; launch dataset contains 91 listings; required static files are present (`index.html`, `app.js`, `CNAME`, `README.md`, `LISTING_PERMISSIONS.md`).
- DNS gate remains external: `CNAME` is set for `abbeynb.com`, but Namecheap/GitHub Pages DNS cutover must be performed and verified in the registrar/DNS UI before claiming launch completion.
- Photo-rights gate remains external for any listing not explicitly approved in `LISTING_PERMISSIONS.md`. Do not re-add Christ in the Desert or Franciscan Renewal Center to the public dataset without new written permission.

## Files
- `index.html` — static HTML shell
- `app.js` — site JavaScript bundle with embedded listings
- `site-listings.json` — launch dataset
