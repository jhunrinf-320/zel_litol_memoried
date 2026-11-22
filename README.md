# Zel Litol Moment — GitHub Pages edition

A static, local-first scrapbook and camera diary website. No build step or framework installation is required.

## Publish with GitHub Pages

1. Create a new GitHub repository, for example `zel-litol-moment`.
2. Upload **all the files in this folder** to the repository's root (not the ZIP file and not an extra enclosing folder).
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch **main** and folder **/(root)**, then click **Save**.
6. Wait for the Pages deployment to finish. Your site URL will look like `https://YOUR-USERNAME.github.io/zel-litol-moment/`.

## Run locally

Run `python -m http.server 8000` in this folder and open `http://localhost:8000`.

## Important notes

- GitHub Pages hosts the static website; it does not store diary photos or scrapbook projects.
- Photos, diary entries, and editable projects are stored in the browser's IndexedDB on the device/browser where they were created. Use the app's backup/export features regularly.
- Camera access requires permission and a secure context. GitHub Pages uses HTTPS.
- Offline app-shell support is available after the site has been opened successfully online once. Browser storage and service-worker support vary by browser.
- The optional PIN is a local privacy gate, not encryption. It does not protect exported files or provide strong security against someone with device access.
- If you change the site later, update the service-worker cache name in `sw.js` so returning visitors can receive the new app shell.
