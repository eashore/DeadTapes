# Download Site

Static landing page for your app downloads.

## Files

- `index.html` - single page
- `styles.css` - visual styling
- `site-config.js` - app name, version text, and the two download URLs

## Update the download links

Edit `site-config.js` and replace:

- `macUrl`
- `windowsUrl`

with your real public file URLs.

## Recommended hosting setup

Use **Cloudflare Pages** for the site itself.

For the app files, use one of these:

- **Cloudflare R2** with public file URLs
- **GitHub Releases** and link directly to the release assets
- Any other public direct-download URLs

## Deploy to Cloudflare Pages

1. In Cloudflare, open **Workers & Pages**.
2. Create a new **Pages** project.
3. Upload the contents of this `download-site` folder.
4. Attach your custom domain.
5. Make sure the URLs in `site-config.js` point to public downloadable files.

## Suggested app file formats

- macOS: ZIP the `.app` after signing/notarizing it
- Windows: use the published `.exe`
