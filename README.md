# Prayer Times Calendar

A free, browser-based prayer times calendar with Hanafi and Hanbali/standard Asr calculation options.

## Files
- `index.html` — main application
- `manifest.json` — installable web app settings
- `sw.js` — service worker for app-shell caching
- `icon-192.png`, `icon-512.png` — application icons

## Publish with GitHub Pages
1. Upload all files to the repository root.
2. Open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select branch `main` and folder `/ (root)`, then Save.
5. Wait for GitHub Pages to publish the site. Open the published HTTPS address.

## Install
- Android Chrome: open the HTTPS site, use the browser menu → **Install app** or **Add to Home screen**.
- Desktop Chrome/Edge: use the install icon in the address bar or the browser menu → **Install**.

## Important limitations
- Fresh prayer times require an internet connection and use the AlAdhan API.
- The service worker caches the application shell, not live prayer-time API results.
- GPS generally requires HTTPS and user permission.
- City search uses OpenStreetMap Nominatim. Please use it responsibly.
- Confirm prayer times with a local mosque or official authority before relying on them for worship.

## Calculation options
The app passes the selected Asr school to AlAdhan:
- Hanafi: `school=1`
- Hanbali/standard: `school=0`

The Automatic regional method leaves the calculation method to the API's default. Check the returned method and compare it with local practice.

## Third-party services
Prayer-time calculations: AlAdhan API. City geocoding: OpenStreetMap Nominatim. Their services have their own terms and availability.
