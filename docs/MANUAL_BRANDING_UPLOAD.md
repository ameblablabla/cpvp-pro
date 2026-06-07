# CPVP.PRO manual branding upload

## Why this step is manual

The GitHub connector used in this session can write UTF-8 text files, including SVG and JSON. It does not upload binary PNG and ICO files.

A complete branding pack is already prepared separately. Upload these files later through the GitHub web interface or a local Git client.

## Upload target

Create or open:

```text
assets/branding/
```

Upload:

```text
logo.svg
logo-mark.png
favicon.ico
apple-touch-icon.png
og-image.png
social-cover.png
announcement-template.png
story-template.png
```

The repository already contains:

```text
assets/branding/logo-mark.svg
assets/branding/favicon.svg
site.webmanifest
```

## Update after upload

After adding `og-image.png`, add these tags to the `<head>` section of `index.html`:

```html
<meta property="og:image" content="https://cpvp.pro/assets/branding/og-image.png">
<meta name="twitter:image" content="https://cpvp.pro/assets/branding/og-image.png">
<link rel="apple-touch-icon" href="/assets/branding/apple-touch-icon.png">
```

After adding `favicon.ico`, keep the SVG favicon as the primary option and add the compatibility fallback:

```html
<link rel="icon" href="/assets/branding/favicon.ico" sizes="any">
```

## Verification

Check:

- `https://cpvp.pro/assets/branding/favicon.svg`
- `https://cpvp.pro/site.webmanifest`
- `https://cpvp.pro/assets/branding/og-image.png`
- social link preview after deployment
