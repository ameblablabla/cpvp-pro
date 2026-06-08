<div align="center">
  <img src="assets/readme-banner.svg" alt="CPVP.PRO — Crystal PvP Platform" width="100%">
</div>

# CPVP.PRO

**CPVP.PRO** — bilingual Russian-English Crystal PvP community platform for Minecraft Java Edition players.

The project is not limited to tier testing. The first public milestone focuses on learning. Later releases add profiles, notifications, Find Duel, teams, licensed Minecraft account linking, Vanilla CPVP TierList, tester workflows, moderation and forum features.

Current public page: [`cpvp.pro`](https://cpvp.pro/)

## Current status

> **In development** — the full platform is not released yet.

Ready now:

- lightweight GitHub Pages landing page;
- custom domain, SEO metadata and branded `404.html`;
- production branding pack;
- Figma foundations and initial desktop layouts;
- normalized product documentation;
- Vanilla CPVP testing draft;
- Discord OAuth and safe Microsoft OAuth linking requirements;
- learning-first roadmap.

## Product direction

First public release:

```text
Learning catalog
Guide pages
Search and filters
Learning progress
Russian-English localization
Browser-language auto-detection
Navbar language switcher
Discord OAuth sign-in
Basic profiles and settings
Notifications
Paid learning subscription tiers
```

Later releases:

```text
Find Duel
Teams
Minecraft account linking
Vanilla CPVP TierList
Tester panel
Moderation panel
Forum
```

## Vanilla CPVP ladder

```text
LT5 < HT5 < LT4 < HT4 < LT3 < HT3 < LT2 < HT2 < LT1 < HT1
```

Detailed rules: [`docs/rules/VANILLA_TESTING_RULES.md`](docs/rules/VANILLA_TESTING_RULES.md)

## Documentation

Start here: [`docs/README.md`](docs/README.md)

Main sections:

```text
docs/
├── product/
├── rules/
├── operations/
├── design/
├── content/
└── references/
```

Key files:

- [`docs/product/ROADMAP.md`](docs/product/ROADMAP.md)
- [`docs/product/DEVELOPMENT_START_CHECKLIST.md`](docs/product/DEVELOPMENT_START_CHECKLIST.md)
- [`docs/product/TBD_DECISIONS.md`](docs/product/TBD_DECISIONS.md)
- [`docs/operations/ACCOUNT_LINKING.md`](docs/operations/ACCOUNT_LINKING.md)
- [`docs/content/LEARNING_PLAN.md`](docs/content/LEARNING_PLAN.md)
- [`docs/design/DESIGN_SYSTEM.md`](docs/design/DESIGN_SYSTEM.md)

## Design sources

Figma:

[`CPVP.PRO — UI Kit and Product Layouts`](https://www.figma.com/design/7VjJ1bfnfWLSnxIJOTHko9/CPVP.PRO-%E2%80%94-UI-Kit-and-Product-Layouts?node-id=0-1&p=f)

Canva:

- [logo and wordmark](https://www.canva.com/d/i0h_0fPMxTsPaFN)
- [social cover](https://www.canva.com/d/4z_sqetriJFXBbc)
- [announcement post](https://www.canva.com/d/gmSwOh1DreTnhJN)
- [story template](https://www.canva.com/d/q3k1ftX70akt_El)

## Landing page principles

The current landing page intentionally stays lightweight:

- no JavaScript;
- no frameworks;
- no external fonts;
- no external stylesheet;
- responsive mobile layout;
- reduced-motion support;
- favicon pack and manifest;
- Open Graph and Twitter image metadata;
- `robots.txt` and `sitemap.xml`.

## Local preview

```bash
python -m http.server 8080
```

Then open `http://localhost:8080`.

## License

No `LICENSE` file has been selected yet. Until then, the source code is not offered for unrestricted copying, modification or redistribution.
