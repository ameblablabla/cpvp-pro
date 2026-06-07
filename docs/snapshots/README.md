# CPVP.PRO requirements snapshots

This directory stores confirmed product decisions collected before implementation.

Use these files as the temporary source of truth until the full documentation restructure is completed.

## Confirmed snapshots

- [`PRODUCT_REQUIREMENTS_RU_EN.md`](PRODUCT_REQUIREMENTS_RU_EN.md) — product positioning, release priorities, bilingual scope and community direction.
- [`TESTING_REQUIREMENTS.md`](TESTING_REQUIREMENTS.md) — Vanilla CPVP ladder, player states, low-tier testing, skip-tests, high-tier evidence, cooldowns and queues.
- [`ACCOUNT_PROFILE_REQUIREMENTS.md`](ACCOUNT_PROFILE_REQUIREMENTS.md) — Discord login, Microsoft account linking, profile fields, badges and customization direction.
- [`MODERATION_COMMUNITY_REQUIREMENTS.md`](MODERATION_COMMUNITY_REQUIREMENTS.md) — tester roles, moderation direction, Discord, Telegram, Find Duel and teams.
- [`TBD_DECISIONS.md`](TBD_DECISIONS.md) — only unresolved items for the next short questionnaire.

## External references

- [`../references/EXTERNAL_TIER_SYSTEM_REFERENCE.md`](../references/EXTERNAL_TIER_SYSTEM_REFERENCE.md) — external ideas preserved for later adaptation. This file is not an official CPVP.PRO ruleset.

## Next migration step

After the remaining `TBD` questions are answered, move confirmed content into the final structure:

```text
docs/
├── product/
├── rules/
├── operations/
├── design/
├── content/
└── references/
```

Then remove old duplicate files only after verifying that no confirmed requirement has been lost.
