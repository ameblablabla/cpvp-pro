# CPVP.PRO Vanilla testing rules

## Positioning

CPVP.PRO is not only a tier-test service. It is an expanding Crystal PvP community platform with learning materials, player profiles, TierList pages, forum features and community tools.

Tier testing is one important part of the platform. The first supported category is `Vanilla`.

## Platform scope

- Supported game: Minecraft Java Edition.
- Gameplay devices: PC and laptop.
- Mobile website: viewing, applications, profiles, TierList, rules and forum convenience only.
- The first public category: `Vanilla`.
- Players build their own kits according to the Vanilla ruleset. Detailed kit rules will be finalized during implementation.

## Minecraft account linking

A player can submit a tier-test application only when:

1. The user is signed in on CPVP.PRO.
2. A licensed Minecraft Java Edition account is linked.
3. The linked account is verified.

The site must never ask for a Microsoft password, Minecraft password or session token. Account linking must use a safe verification flow. Exact implementation will be selected during development.

The purpose of account linking is identity verification and accountability, not access to the player's Minecraft account.

## Full tier ladder

From lowest to highest:

```text
LT5
HT5
LT4
HT4
LT3
HT3
LT2
HT2
LT1
HT1
```

Compact notation:

```text
LT5 < HT5 < LT4 < HT4 < LT3 < HT3 < LT2 < HT2 < LT1 < HT1
```

## League split

### Low tiers

```text
LT5
HT5
LT4
HT4
LT3
```

Low-tier applications are tested by regular testers.

### High tiers

```text
HT3
LT2
HT2
LT1
HT1
```

High-tier tests are played against real ranked players close to the target level.

## Match format

- Standard match format: `First to 4`.
- Players continue until one player reaches four wins.
- Possible final scores: `4:0`, `4:1`, `4:2`, `4:3`.
- For high-tier tests, both players agree on the server before the match.
- For low-tier tests, the tester and applicant also agree on the server before the match.

## Low-tier test flow

A regular tester evaluates the applicant by gameplay and should be experienced enough to estimate the player's approximate tier from the match.

Rules:

1. The applicant plays against a regular tester.
2. The regular tester may assign a result up to `LT3`.
3. A normal low-tier test cannot directly award `HT3` or higher.
4. A player may submit a new tier-test application once per week.

## Bonus HT3 skip-test

A strong low-tier applicant may receive a chance to test for `HT3` immediately.

Qualification:

```text
4:0
or
4:1
```

These scores represent at least 75% wins in a First to 4 match.

Flow:

1. The applicant plays a regular tester.
2. If the applicant wins `4:0` or `4:1`, the applicant receives an HT3 skip-test opportunity.
3. The bonus HT3 test is played against a senior tester.
4. If the applicant wins the senior tester match, the applicant receives `HT3`.

## Regular testers

Requirements:

- minimum rank: `LT3`;
- selected through tester recruitment;
- approved and added by staff;
- trusted by the project team.

Responsibilities:

- conduct low-tier tests;
- estimate the applicant's approximate tier from gameplay;
- issue low-tier results up to `LT3`;
- identify applicants eligible for the HT3 skip-test;
- record the result and brief reason.

## Senior testers

Senior testers are not automatically assigned to every `HT3` player.

Requirements:

- already be a regular tester;
- receive `HT3` or higher;
- be selected by staff as suitable for the role;
- remain trusted and consistent.

Responsibilities:

- conduct bonus HT3 skip-tests;
- spectate high-tier matches when needed;
- review full recordings;
- provide quick verdicts;
- participate in disagreement resolution.

## High-tier tests

For `HT3+`, the applicant plays against a real ranked player.

Opponent selection rule:

- the opponent must be in the same tier or no more than one ladder step above or below the target tier;
- low-tier and high-tier league boundaries must still be respected.

Example:

- an `HT3` player may play against `HT3` or `LT2`;
- an `HT3` player may not use `LT3` as an opponent because `LT3` belongs to the low-tier league.

## High-tier evidence requirements

For a normal `HT3+` test, use one of two verification methods.

### Option A — Full recording

At least one participant records the complete match.

Requirements:

- recording begins before joining the agreed server;
- the agreed IP address is visible during direct connection;
- the Minecraft username is visible;
- the full fight is recorded;
- the recording is uncut;
- the hotbar and normal gameplay HUD remain visible;
- the complete original recording must be available for review;
- one or both players may submit recordings.

### Option B — Senior tester spectator

A senior tester spectates the match and observes the full fight.

Requirements:

- the server is agreed in advance;
- the senior tester observes the complete match;
- the senior tester records the result and notes.

## Recording verdicts

When recordings are used instead of a senior tester spectator:

1. At least two senior testers review the full recording.
2. They should provide a quick verdict.
3. If both agree, the verdict is accepted.
4. If they disagree, staff resolves the case.

## High-tier progression reference

The exact phase structure for `LT2`, `HT2`, `LT1` and `HT1` will be finalized during implementation.

Current reference model:

### Testing for HT3

- Phase 1: qualify through tester evaluation or existing high-tier progression.
- Phase 2: beat an `HT3` opponent in the required match format.

### Testing for LT2 / HT2

- Beat opponents close to the applicant's current tier.
- Achieve a sufficient score against opponents in the target tier.

### Testing for LT1

- Beat lower high-tier opponents.
- Beat opponents close to the applicant's current tier.
- Achieve a sufficient overall score against target-tier players.

### Testing for HT1

- Beat required lower high-tier opponents.
- Beat required `HT2` opponents.
- Beat opponents in the applicant's current tier.
- Beat the current `HT1` title holder to take the title.

## Cooldown

- A player may submit a tier-test application once per week.
- The exact cooldown timestamp behavior will be implemented in backend rules.

## Rules still to finalize during implementation

- detailed Vanilla kit rules;
- exact phase requirements for `LT2`, `HT2`, `LT1`, `HT1`;
- biome striking rules;
- cross-region and ping equalization rules;
- allowed and disallowed mods;
- anti-cheating policy details;
- appeal flow details;
- exact evidence upload format;
- storage and retention rules for recordings.
