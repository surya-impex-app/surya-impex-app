SURYA IMPEX MOBILE APP (PWA)

This package is prepared for an installable, app-like mobile experience.

Files:
- Index.html = mobile app
- manifest.json = app/install settings
- sw.js = offline/app shell
- icon.svg = SURYA IMPEX app icon

IMPORTANT:
A true installable PWA must be served from a normal HTTPS website.
The Google Apps Script URL is kept as the Google Sheets/Drive backend.
Do NOT open Index.html using content:// on the phone.

After the frontend is hosted on HTTPS:
1. Open the HTTPS link in Chrome on Android.
2. Tap the browser menu.
3. Choose "Install app" or "Add to Home screen".
4. Launch SURYA IMPEX from the phone icon.

Google Apps Script:
- Keep your existing Code.gs backend.
- The existing /exec URL remains the backend.
- The app should use the existing backend bridge/API after the frontend is hosted.

Camera:
- Scan buttons use the phone camera/photo capture path rather than relying on
  getUserMedia inside an Apps Script iframe.
