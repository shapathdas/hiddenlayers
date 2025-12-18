# Hidden Layers Landing Page

A simple, static site for the Hidden Layers Reading Group. It mirrors the reference designs with a green hero, layered cream/white content sections, and a fixed pill-style header. Footer includes partner logos and quick links.

## Features
- Fixed, rounded header with nav and CTA.
- Full-height green hero with large headline.
- White content sections: Frontier List, Methodology.
- Footer with three logo slots (linked), social links, and quick links.
- Favicon + social preview (Open Graph + Twitter cards) using the Hidden Layers logo.

## Tech
- Pure HTML + CSS (Inter font from Google Fonts).
- No build step or dependencies.

## File Structure
- `index.html` — markup and meta tags for favicon/OG/Twitter.
- `styles.css` — layout, typography, responsive tweaks.
- Assets: `Logo_HDLR_typeStyle.png` (also used for favicon/social), `Logo_HDLR_typeStyle.svg`, `Logo_HDLR_typeStyle_2.jpg`, `Web_FRLST.png`, `Attached_image.png` (IIITB logo).

## Running Locally
Open `index.html` directly in a browser, or serve the folder:
```bash
cd /Users/shapathdas/Developer/HDLR
python -m http.server 3000
# then visit http://localhost:3000
```

## Deployment

### Firebase Hosting
This site is deployed to Firebase Hosting at **https://hdlr2025.web.app**

To deploy:
```bash
firebase deploy --only hosting
```

The Firebase project is configured in:
- `firebase.json` - Hosting configuration
- `.firebaserc` - Project ID (hdlr2025)

### Other Hosting Options
Any static host (GitHub Pages, Netlify, Vercel, S3). Upload the contents of this folder; no build needed.

## Updating Logos/Links
- Footer logos live in `index.html` under `.footer__logos`. Replace `img` sources and `href` targets as needed.
- Social links are in `.footer__links`. Quick links in `.footer__nav`.

## Meta Preview
- Favicon: `Logo_HDLR_typeStyle.png`
- OG/Twitter image: `Logo_HDLR_typeStyle.png`
- Title/description set in `<head>` of `index.html`.

