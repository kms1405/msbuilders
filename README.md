# BuildLog — Static Construction Website

A responsive two-page website for documenting a home construction project. It uses plain HTML, CSS and JavaScript, so it can be hosted free with GitHub Pages. No backend or build tools are required.

## Pages
- `index.html` — home page, construction topics, site address and contact details.
- `gallery.html` — photo gallery with category filters and embedded YouTube video slots.

## Before publishing: personalize the content

### 1. Contact details
Open `index.html` and replace:
- `+91 XXXXX XXXXXX` with your phone number (also update the `tel:` link).
- `yourname@example.com` with your email address (also update the `mailto:` link).
- Edit the site address if you want to show a more precise address.

### 2. Add your construction photos
Copy your photos into the `assets` folder and name them:
- `site-01.jpg`
- `site-02.jpg`
- `site-03.jpg`
- `site-04.jpg`
- `site-05.jpg`
- `site-06.jpg`

You can use `.jpg`, `.png` or `.webp`, but if you change the extension, update the matching `src` in `gallery.html`. The gallery currently displays designed placeholders until the matching image files are added. For best results, use landscape photos around 1200 × 800 pixels.

### 3. Add YouTube videos
Open `gallery.html`. Find the two iframe URLs:
- `https://www.youtube-nocookie.com/embed/VIDEO_ID_1`
- `https://www.youtube-nocookie.com/embed/VIDEO_ID_2`

Replace each `VIDEO_ID_1` / `VIDEO_ID_2` with the ID from your YouTube video URL. Example: for `https://www.youtube.com/watch?v=AbCd1234`, the ID is `AbCd1234`. For a YouTube Shorts link, use the ID after `/shorts/`.

To add more photos or videos, duplicate an existing card and update its filename, title and category.

## Publish using GitHub Pages
1. Sign in to GitHub and create a new **public** repository, for example `construction-site`.
2. Upload all files and folders from this project. Keep `index.html`, `gallery.html`, `style.css` and `script.js` in the repository root. Keep photos inside `assets/`.
3. Open the repository **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Choose branch `main` and folder `/ (root)`, then click **Save**.
6. Wait for the deployment to finish. Your website address will look like `https://YOUR-USERNAME.github.io/construction-site/`.

If you use a custom domain later, configure it under Settings → Pages.

## Notes
- This is a static website: it does not collect form submissions or store visitor data.
- The map link opens a Google Maps search for the site area.
- The hero section uses externally hosted Unsplash photos; a network connection is needed to load them. The rest of the site is local.
- Google Fonts are also loaded online; the site falls back to system fonts if unavailable.
