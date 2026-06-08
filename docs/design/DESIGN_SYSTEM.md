# CPVP.PRO design system

## Direction

CPVP.PRO uses a premium dark gaming interface with restrained blue and violet accents, clear spacing, responsive layouts and moderate visual effects.

## Core tokens

| Token | Value |
|---|---|
| Background | `#05070D` |
| Surface | `#0D111E` |
| Muted surface | `#141A2B` |
| Primary text | `#EEF4FF` |
| Secondary text | `#9AA7BD` |
| Blue accent | `#72D7FF` |
| Violet accent | `#9B6CFF` |
| Active status | `#94FFCF` |
| Warning | `#FF7C92` |

Spacing scale:

```text
4 8 12 16 24 32 48 64
```

Radii:

```text
12px 18px 26px 999px
```

## Production rules

- Prefer system fonts.
- Avoid unnecessary external dependencies.
- Animate with `transform` and `opacity` where possible.
- Support `prefers-reduced-motion`.
- Keep focus states visible.
- Do not use color as the only status signal.
- Avoid horizontal scrolling on mobile.

## Core UI

Required component groups:

- navigation and language switcher;
- buttons;
- cards for guides, players, tiers, teams and moderation cases;
- forms and validation;
- status badges;
- loading, empty and error states;
- modals and notifications.

## Profile customization

Customization starts at `HT3+` and becomes stronger at higher tiers.

Suggested progression:

```text
HT3+: accent color, frame, banner
LT2+: animated border, featured match, badge layout
HT2+: advanced effects, featured guide, more highlight slots
LT1+: premium theme, rare frame set, expanded highlights
HT1: exclusive champion-style visual package
```

Paid learning subscriptions also unlock top-level profile customization comparable to HT1. Rank-based and subscription-based cosmetics should remain visually distinguishable.

## Figma

Main editable file:

[`CPVP.PRO — UI Kit and Product Layouts`](https://www.figma.com/design/7VjJ1bfnfWLSnxIJOTHko9/CPVP.PRO-%E2%80%94-UI-Kit-and-Product-Layouts?node-id=0-1&p=f)

Ready:

- cover;
- foundations;
- base UI-kit;
- desktop home;
- desktop learning;
- desktop TierList;
- desktop forum.

Next:

- mobile layouts;
- desktop player profile;
- desktop moderation queue;
- final visual review.

## Canva and branding

Editable Canva sources:

- [logo and wordmark](https://www.canva.com/d/i0h_0fPMxTsPaFN)
- [social cover](https://www.canva.com/d/4z_sqetriJFXBbc)
- [announcement post](https://www.canva.com/d/gmSwOh1DreTnhJN)
- [story template](https://www.canva.com/d/q3k1ftX70akt_El)

Production assets are stored in `assets/branding/`.
