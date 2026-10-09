PACEPILOT — Android installable web app
======================================

IMPORTANT
This is a Progressive Web App (PWA), not a signed Android APK. Install it on Android by hosting these files on an HTTPS website. Geolocation and install prompts generally require HTTPS (localhost is an exception).

QUICK DEPLOY WITH GITHUB PAGES
1. Sign in to GitHub and create a new public repository, for example pacepilot.
2. Upload index.html, manifest.webmanifest, sw.js, and icon.svg to the repository root.
3. In the repository, open Settings > Pages.
4. Under Build and deployment, choose Deploy from a branch, select main and /(root), then Save.
5. Wait for the published HTTPS URL shown in Pages.
6. Open that URL in Chrome on your Android phone.
7. Allow Location permission. For the best GPS results, enable precise location and keep the phone outdoors or near a clear view of the sky.
8. In Chrome, tap ⋮ > Add to Home screen (or Install app, if shown). Open PACEPILOT from the home screen.

FEATURES
- Red screen/dial until current GPS pace is at or faster than target; green at target or faster.
- Clock dial: target at 12 o'clock, faster clockwise, slower counterclockwise.
- GPS location map, route trace and heading arrow where the device provides heading.
- Expand/shrink map and dial independently.
- Elapsed time, GPS distance, current pace and average pace.
- Best-effort motion-sensor step estimate.

LIMITATIONS
- This is a browser-based PWA, not an APK. The map requires internet and uses CARTO Voyager basemap tiles (with OpenStreetMap data) through Leaflet. If tiles still fail on a network, check whether that network blocks the tile host.
- Location permission and a secure HTTPS host are required for GPS.
- Step estimates require motion-sensor data exposed by the phone/browser and are not medical-grade or guaranteed accurate.
- Heading arrow rotates when GPS heading is available; stationary or low-speed heading may be unavailable.
- Pace is calculated from GPS and may jump with poor signal or very short distances.
- Do not interact with the screen while running; secure the phone and follow local safety rules.
