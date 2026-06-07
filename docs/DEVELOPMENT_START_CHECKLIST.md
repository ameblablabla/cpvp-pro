# CPVP.PRO development start checklist

## Product position

CPVP.PRO is an expanding Crystal PvP community platform.

The platform includes:

- learning materials;
- player profiles;
- forum and community tools;
- TierList pages;
- Vanilla tier testing;
- moderation and appeals;
- news and announcements.

Tier testing is an important feature, but it is not the whole product.

## Decisions already fixed

### Initial category

```text
Vanilla
```

### Supported game

```text
Minecraft Java Edition
PC and laptop gameplay only
```

The mobile site is for convenient access to profiles, TierList, rules, applications, forum and news.

### Tier ladder

```text
LT5 < HT5 < LT4 < HT4 < LT3 < HT3 < LT2 < HT2 < LT1 < HT1
```

### League split

Low-tier league:

```text
LT5
HT5
LT4
HT4
LT3
```

High-tier league:

```text
HT3
LT2
HT2
LT1
HT1
```

### Match format

```text
First to 4
```

### Low-tier testing

- conducted by regular testers;
- tester estimates approximate tier from gameplay;
- maximum normal award: `LT3`;
- test cooldown: one application per week.

### HT3 skip-test

Qualifying regular tester scores:

```text
4:0
4:1
```

The bonus test is played against a senior tester. A win grants `HT3`.

### High-tier testing

- played against real ranked players close to the target tier;
- server agreed before the match;
- full recording or senior tester spectator verification required;
- recordings reviewed by at least two senior testers;
- staff resolves disagreement.

### Minecraft account linking

Tier-test applications require:

```text
signed-in user
linked Minecraft Java Edition account
verified account ownership
```

The website must never request a Microsoft password, Minecraft password or session token.

## Implementation order

### Phase 1 — Project foundation

- [ ] Choose frontend stack.
- [ ] Choose backend stack.
- [ ] Choose database.
- [ ] Create development environment.
- [ ] Define environment variables.
- [ ] Add local development instructions.
- [ ] Add staging deployment.

### Phase 2 — Authentication and identity

- [ ] Add site account registration and sign in.
- [ ] Add user profile.
- [ ] Implement safe Minecraft account linking.
- [ ] Add unlink flow.
- [ ] Add verified player status.
- [ ] Add role model.

### Phase 3 — Community core

- [ ] Add public profiles.
- [ ] Add news and announcements.
- [ ] Add forum categories.
- [ ] Add forum topics and replies.
- [ ] Add reports.
- [ ] Add notifications.

### Phase 4 — Learning section

- [ ] Add learning categories.
- [ ] Add guide pages.
- [ ] Add search and filters.
- [ ] Add progress tracking.

### Phase 5 — Vanilla TierList

- [ ] Add Vanilla category.
- [ ] Add tier ladder.
- [ ] Add player rank history.
- [ ] Add public TierList page.
- [ ] Add tier-test application form.
- [ ] Add weekly cooldown.
- [ ] Add tester queue.
- [ ] Add result entry.
- [ ] Add HT3 skip-test flow.
- [ ] Add high-tier evidence review.
- [ ] Add appeals.

### Phase 6 — Moderation

- [ ] Add staff role management.
- [ ] Add regular tester recruitment workflow.
- [ ] Add senior tester appointment workflow.
- [ ] Add moderation queue.
- [ ] Add review notes.
- [ ] Add action history.
- [ ] Add staff disagreement resolution.

### Phase 7 — Quality

- [ ] Add error monitoring.
- [ ] Add performance monitoring.
- [ ] Add backup strategy.
- [ ] Add rate limiting.
- [ ] Add file upload validation.
- [ ] Review accessibility.
- [ ] Run closed testing.

## Details intentionally postponed until implementation

- detailed Vanilla kit rules;
- exact phase requirements for `LT2`, `HT2`, `LT1`, `HT1`;
- biome striking;
- cross-region rules;
- ping equalization;
- allowed and disallowed mods;
- evidence upload storage;
- recording retention;
- appeal limits;
- anti-cheating enforcement details.

## First task when development starts

Before writing feature code:

1. Review this checklist.
2. Review [`VANILLA_TESTING_RULES.md`](VANILLA_TESTING_RULES.md).
3. Review [`ACCOUNT_LINKING.md`](ACCOUNT_LINKING.md).
4. Choose the stack.
5. Create the first architecture branch.
