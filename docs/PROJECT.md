# CPVP.PRO project overview

## Product position

CPVP.PRO is an expanding Crystal PvP community platform.

The project is not limited to tier testing. It is intended to combine:

- learning materials;
- player profiles;
- Vanilla TierList pages;
- tier-test applications;
- forum and community tools;
- news and announcements;
- moderation and appeals.

## Current public version

CPVP.PRO currently uses a lightweight static landing page published through GitHub Pages.

## Current files

- `index.html` contains the landing page markup and inline styles.
- `404.html` contains the fallback page.
- `CNAME` connects the custom domain.
- `assets/branding/` contains the production branding pack.
- `assets/readme-banner.svg` is used in the repository README.
- `site.webmanifest` contains the site icons and theme metadata.

## First competitive category

```text
Vanilla
```

The first release should support only Vanilla Crystal PvP. Detailed kit rules will be finalized during implementation.

## Product principles

- Keep the first load fast.
- Avoid unnecessary dependencies.
- Check desktop and mobile layouts.
- Keep visual effects moderate.
- Document structural changes.
- Treat tier testing as one feature of a larger community platform.
- Use safe Minecraft account verification without collecting passwords or tokens.

## Requirements already fixed

- Minecraft Java Edition only.
- PC and laptop gameplay only.
- Mobile site for convenient access, not gameplay.
- Safe linked Minecraft account required for tier-test applications.
- Vanilla ladder from `LT5` to `HT1`.
- Low-tier and high-tier league split.
- First to 4 match format.
- Weekly application cooldown.
- Regular tester and senior tester roles.
- Full recording or senior tester spectator verification for high-tier tests.
- At least two senior tester verdicts for recorded high-tier matches.
- Staff resolves senior tester disagreement.

## Development entry point

When implementation begins:

1. Review [`DEVELOPMENT_START_CHECKLIST.md`](DEVELOPMENT_START_CHECKLIST.md).
2. Review [`VANILLA_TESTING_RULES.md`](VANILLA_TESTING_RULES.md).
3. Review [`ACCOUNT_LINKING.md`](ACCOUNT_LINKING.md).
4. Choose the stack.
5. Create the first architecture branch.
