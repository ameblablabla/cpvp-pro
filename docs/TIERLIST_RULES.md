# CPVP.PRO TierList rules

## Product role

TierList is one part of CPVP.PRO. The platform itself is an expanding Crystal PvP community with learning materials, player profiles, forum features and community tools.

The first supported competitive category is `Vanilla`.

Detailed testing rules are stored in [`VANILLA_TESTING_RULES.md`](VANILLA_TESTING_RULES.md).

## Category

```text
Vanilla
```

Players build their own kits according to the Vanilla ruleset. Detailed kit restrictions will be finalized during implementation.

## Full ladder

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

### Low-tier league

```text
LT5
HT5
LT4
HT4
LT3
```

Low-tier tests are conducted by regular testers. A regular tester may award a result up to `LT3`.

### High-tier league

```text
HT3
LT2
HT2
LT1
HT1
```

High-tier tests are played against real ranked players close to the target tier.

## High-tier opponent selection

- The opponent must be in the same tier or no more than one ladder step above or below the target tier.
- Low-tier and high-tier league boundaries must still be respected.

Example:

- an `HT3` applicant may play against `HT3` or `LT2`;
- an `HT3` applicant may not play against `LT3`, because `LT3` belongs to the low-tier league.

## Match format

```text
First to 4
```

Players continue until one participant reaches four wins.

Possible final scores:

```text
4:0
4:1
4:2
4:3
```

## Low-tier evaluation

A regular tester evaluates the applicant by gameplay and should be experienced enough to estimate the player's approximate tier from the match.

Rules:

1. The applicant plays a regular tester.
2. The regular tester records the result and a brief reason.
3. The regular tester may assign a result up to `LT3`.
4. A normal low-tier test cannot award `HT3` or higher directly.

## Bonus HT3 skip-test

If the applicant beats a regular tester with at least 75% wins in a First to 4 match, the applicant receives an HT3 skip-test opportunity.

Qualifying scores:

```text
4:0
4:1
```

The bonus test is played against a senior tester. If the applicant wins, the applicant receives `HT3`.

## High-tier verification

For a normal `HT3+` test, use one of two methods:

1. Full recording from at least one participant.
2. Full-match observation by a senior tester in spectator mode.

When recordings are used:

- at least two senior testers review the full recording;
- if both agree, the verdict is accepted;
- if they disagree, staff resolves the case.

## Cooldown

A player may submit a tier-test application once per week.

## Application requirements

A tier-test application is available only to users who:

1. are signed in on CPVP.PRO;
2. linked a licensed Minecraft Java Edition account;
3. completed safe account verification.

The site must never ask for a Microsoft password, Minecraft password or session token.

## Still to finalize during implementation

- detailed Vanilla kit rules;
- exact phase requirements for `LT2`, `HT2`, `LT1`, `HT1`;
- biome striking rules;
- cross-region and ping equalization rules;
- allowed and disallowed mods;
- anti-cheating policy details;
- evidence upload format;
- appeal flow details.
