# CPVP.PRO branding status

## Canva source designs

Editable Canva sources:

- Logo and wordmark: https://www.canva.com/d/i0h_0fPMxTsPaFN
- Social cover: https://www.canva.com/d/4z_sqetriJFXBbc
- Announcement post: https://www.canva.com/d/gmSwOh1DreTnhJN
- Story template: https://www.canva.com/d/q3k1ftX70akt_El

## Added to the repository

- [x] `assets/branding/logo-mark.svg`
- [x] `assets/branding/favicon.svg`
- [x] `site.webmanifest`
- [x] Production favicon SVG connected in `index.html`
- [x] Webmanifest connected in `index.html`

## Ready in the branding pack but not uploaded automatically

The GitHub connector used in this session accepts UTF-8 text files, but it does not upload binary files. The following exports are ready and must be uploaded manually later:

```text
assets/branding/
├── logo.svg
├── logo-mark.png
├── favicon.ico
├── apple-touch-icon.png
├── og-image.png
├── social-cover.png
├── announcement-template.png
└── story-template.png
```

## Recommended upload order

1. `og-image.png`
2. `apple-touch-icon.png`
3. `favicon.ico`
4. `logo.svg`
5. Social templates

After uploading `og-image.png`, add these tags to `index.html`:

```html
<meta property="og:image" content="https://cpvp.pro/assets/branding/og-image.png">
<meta name="twitter:image" content="https://cpvp.pro/assets/branding/og-image.png">
```

## Export rules

- Prefer SVG for logo and logo mark.
- Use PNG and ICO for compatibility where needed.
- Keep `og-image.png` at `1200×630`.
- Keep social exports optimized for web use.
- Avoid external font dependencies in production assets.
