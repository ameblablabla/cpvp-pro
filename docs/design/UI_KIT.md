# CPVP.PRO UI kit specification

## Tokens

### Colors

| Token | Value | Usage |
|---|---|---|
| `--bg` | `#05070D` | Main background |
| `--surface` | `#0D111E` | Cards and panels |
| `--surface-muted` | `#141A2B` | Secondary surface |
| `--line` | `rgba(150,180,255,.15)` | Borders |
| `--text` | `#EEF4FF` | Primary text |
| `--muted` | `#9AA7BD` | Secondary text |
| `--blue` | `#72D7FF` | Main accent |
| `--violet` | `#9B6CFF` | Supporting accent |
| `--green` | `#94FFCF` | Active status |
| `--danger` | `#FF7C92` | Errors and warnings |

### Radii

```text
12px
18px
26px
999px
```

### Spacing

```text
4 8 12 16 24 32 48 64
```

## Components

### Navigation

- desktop navbar;
- mobile top bar;
- mobile drawer;
- breadcrumbs;
- tabs;
- language switcher.

### Buttons

- primary;
- secondary;
- ghost;
- danger;
- icon button.

All buttons need `default`, `hover`, `focus-visible`, `disabled` and `loading` states.

### Cards

- feature card;
- guide card;
- player card;
- tier card;
- team card;
- Find Duel card;
- profile stat card;
- moderation case card;
- subscription tier card.

### Forms

- text input;
- search input;
- textarea;
- select;
- checkbox;
- radio;
- switch;
- validation message.

### Feedback

- status badge;
- tier badge;
- punishment badge with hover details;
- Retired badge;
- Inactive badge;
- toast;
- empty state;
- loading skeleton;
- inline alert;
- confirmation modal.

## Page templates

- home;
- learning catalog;
- guide page;
- player profile;
- account settings;
- subscriptions;
- Find Duel;
- team page;
- TierList;
- tester panel;
- moderation queue;
- forum category;
- forum topic.

## Accessibility

- visible `focus-visible` states;
- status must not rely on color alone;
- icon-only controls need `aria-label`;
- dark-theme contrast must remain readable;
- animation must respect `prefers-reduced-motion`.
