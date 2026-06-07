# CPVP.PRO visual language

## Direction

CPVP.PRO should feel like a focused premium gaming platform rather than a generic Minecraft website.

The interface should use:

- dark backgrounds;
- clear spacing and grid alignment;
- restrained neon accents;
- glass-like cards only where they help hierarchy;
- compact technical labels;
- strong typography on hero sections;
- responsive layouts for desktop and mobile.

## Color palette

| Token | Value | Usage |
|---|---|---|
| Background | `#05070D` | Main page background |
| Surface | `#0D111E` | Cards and panels |
| Text | `#EEF4FF` | Primary text |
| Muted | `#9AA7BD` | Secondary text |
| Blue accent | `#72D7FF` | Highlights and focus states |
| Violet accent | `#9B6CFF` | Supporting gradients |
| Green status | `#94FFCF` | Online and active states |

## Typography

Use system fonts by default for production performance. Design mockups may use similar geometric sans-serif fonts, but exported assets should not require external font loading unless there is a clear reason.

Recommended production stacks:

```css
font-family: Inter, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
font-family: ui-monospace, SFMono-Regular, Menlo, Consolas, monospace;
```

## Layout rules

- Keep content width limited and centered.
- Use large visual spacing in hero sections.
- Prefer 8px-based spacing increments.
- Keep cards simple and avoid excessive blur.
- Use one or two accent colors per block.
- Keep mobile layouts readable without horizontal scrolling.

## Motion rules

- Prefer `transform` and `opacity` for animations.
- Avoid animations that continuously change layout dimensions.
- Disable non-essential motion on mobile when it improves performance.
- Respect `prefers-reduced-motion`.

## Figma source

Main editable Figma file:

[`CPVP.PRO — UI Kit and Product Layouts`](https://www.figma.com/design/7VjJ1bfnfWLSnxIJOTHko9/CPVP.PRO-%E2%80%94-UI-Kit-and-Product-Layouts?node-id=0-1&p=f)

Current Figma status is documented in [`FIGMA_STATUS.md`](FIGMA_STATUS.md).

## Canva sources

Editable Canva source designs:

- [logo and wordmark](https://www.canva.com/d/i0h_0fPMxTsPaFN);
- [wide social cover](https://www.canva.com/d/4z_sqetriJFXBbc);
- [square announcement post](https://www.canva.com/d/gmSwOh1DreTnhJN);
- [vertical story template](https://www.canva.com/d/q3k1ftX70akt_El).

Current export status is documented in [`BRANDING_STATUS.md`](BRANDING_STATUS.md).

## Figma and Canva workflow

Figma or Canva can be used for concept work, banners, social visuals and UI exploration. Keep source design files outside the production path unless the team intentionally publishes them.

For repository assets:

- export optimized SVG when possible;
- use WebP or AVIF for raster images;
- avoid oversized exports;
- keep filenames descriptive;
- do not embed external font dependencies into production pages.
