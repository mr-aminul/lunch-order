# Lunch order (static page)

Single-page lunch order form: Google sign-in, meal choices, cancel. Orders post to Google Sheets via Apps Script.

## Setup

1. Open `index.html` in an editor and set `GOOGLE_CLIENT_ID` and `APPS_SCRIPT_WEB_APP_URL` in the `<script>` block.
2. Serve the folder over **HTTPS** (or `http://localhost`) so Google Sign-In works — not `file://`.
3. Deploy your Apps Script web app (POST handler) as described in the comments inside `index.html`.

## GitHub Pages

Repository **Settings → Pages**: source **Deploy from a branch**, branch **main** and folder **/ (root)**. The app will be at `https://<user>.github.io/<repo>/`.

Add your GitHub Pages URL to the OAuth client **Authorized JavaScript origins** in Google Cloud Console.
