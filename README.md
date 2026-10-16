# WBTP

Public website for wontbetold Productions, live at https://wontbetold.com.

Static HTML, no build step. Hosted on Vercel, deployed automatically from `main`.

## Pages

- `index.html` home and contact form, at /
- `company.html` the company, at /company
- `work.html` films, theatre, commercials and music videos, at /work
- `christapor.html` founder, at /christapor
- `privacy.html` privacy policy, at /privacy

## Other files

- `logo.png`, `lips.png`, `wordmark.png` brand artwork
- `images/` photos, posters and stills used on the pages
- `favicon.png`, `apple-touch-icon.png`, `og-image.png` icons and link preview
- `vercel.json` clean URLs (pages are served without .html)
- `robots.txt`, `sitemap.xml`, `llms.txt` search and AI visibility
- `sitemap-for-launch.xml` the sitemap to use once /company, /work and /christapor are set to index (see below)

## Contact form

The form posts to Formspree. Replace `YOUR_FORM_ID` in `index.html` with the form ID from the Formspree dashboard.

## Google Analytics

The GA4 snippet is in the `<head>` of every page. Replace `G-XXXXXXXXXX` (two places per page, five pages) with the Measurement ID from the GA4 property.

## Launch

1. Allow wontbetold.com (and the vercel.app preview domain, for testing) in the embed settings of each Vimeo video.
2. In `company.html`, `work.html` and `christapor.html`, change `noindex,follow` to `index,follow`.
3. Replace the contents of `sitemap.xml` with `sitemap-for-launch.xml`.

## Editing

Edit the file on GitHub, commit to `main`. Vercel redeploys in about a minute. The company name is always "wontbetold Productions", lowercase w.
