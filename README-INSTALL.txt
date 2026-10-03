PROJECT PASHA'S LVL UP — PWA PACKAGE

Files:
- index.html       Main tracker
- manifest.webmanifest  App name, icon, standalone behavior
- sw.js            Offline cache/service worker
- icons/           192px and 512px app icons

IMPORTANT:
A PWA must be served from HTTPS (or localhost during development) to be installable. Opening index.html directly as a file will NOT give Chrome the normal PWA install flow.

Recommended deployment:
1. Upload this folder to a static HTTPS host (for example GitHub Pages, Netlify, or Vercel).
2. Open the HTTPS URL in Chrome on the Samsung A15.
3. Chrome should offer Install app / Add to Home screen. You can also use the in-app Install App button when the browser exposes the install prompt.
4. After installation, launch it from the app icon. It opens in standalone mode without the normal Chrome address bar.

The tracker still stores daily data in browser localStorage on the device. Installing the PWA does not automatically move old data from a different browser/origin; data is origin-specific.
