# CPVP.PRO Vanilla testing rules

## Positioning

CPVP.PRO is not only a tier-test service. It is an expanding Crystal PvP community platform with learning materials, player profiles, TierList pages, forum features and community tools.

Tier testing is one important part of the platform. The first supported category is `Vanilla CPVP`.

## Platform scope

- Supported game: Minecraft Java Edition.
- Gameplay devices: PC and laptop.
- Mobile website: viewing, applications, profiles, TierList, rules and forum convenience only.
- The first public category: `Vanilla CPVP`.
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

## Player ranking states

### Unranked

A player may have no tier. The profile shows:

```text
Unranked
```

Confirmed access for an Unranked player:

- forum participation;
- Find Duel access;
- team features;
- following players;
- guide comments.

Other access restrictions remain `TBD` until implementation.

### Retired

A ranked player may freeze the current tier by entering `Retired` status.

Rules:

- the player enables Retired voluntarily;
- a reason is required;
- the minimum Retired period is three months;
- a Retired player cannot participate in tier tests;
- after leaving Retired, the player must complete a retest;
- Retired tiers use the `R` prefix;
- a public Retired badge is shown.

Examples:

```text
RLT3
RHT5
RHT3
```

### Inactive

Monthly activity requirements apply only to `HT3+` players.

Rules:

- an `HT3+` player must complete at least one official test per month or enter Retired status;
- frequent reminders should be sent before the activity deadline;
- if the player misses the deadline, the profile receives `Inactive` status;
- the player's tier is lowered to `LT3` regardless of the previous high-tier rank.

### Restricted

Restricted is a disciplinary state.

Confirmed escalation:

```text
First Restricted: 1 month
Second Restricted: 90 days
Third Restricted: permanent project ban
```

Rules:

- the player's tiers are reset;
- the previous tier history remains visible;
- the Restricted badge remains permanently visible in the profile history;
- the player may appeal a Restricted decision;
- after a temporary Restricted period ends, the player returns as `Unranked`.

Detailed violation mapping remains `TBD` until the anti-cheating and moderation rules are finalized.

## Match format

- Standard match format: `First to 4`.
- Players continue until one player reaches four wins.
- Possible final scores: `4:0`, `4:1`, `4:2`, `4:3`.
- For high-tier tests, both players agree on the server before the match.
- For low-tier tests, the tester and applicant also agree on the server before the match.

## Waitlist and application flow

### Low-tier waitlist

1. The player submits an application.
2. The player is added to a waitlist channel.
3. A tester of the requested region starts a queue when available.
4. Players in the waitlist are pinged.
5. The player joins the queue and completes the test.

Required application data:

- region of the server where the player wants to test;
- Minecraft username used for the test;
- preferred time;
- preferred server.

Providing false information results in a denied test.

### High-tier applications

If the player is `HT3` or higher, a high-ticket flow is created instead of the low-tier waitlist flow.

Detailed ticket implementation remains `TBD` until development.

## Low-tier test flow

A regular tester evaluates the applicant by gameplay and should be experienced enough to estimate the player's approximate tier from the match.

Rules:

1. The applicant plays against a regular tester.
2. The regular tester chooses the resulting low-tier rank based on actual gameplay.
3. The regular tester may assign any low-tier rank from `LT5` to `LT3`.
4. `LT5` is the minimum tier.
5. The match score does not automatically determine the low-tier rank.
6. A player may lose the match and still receive `LT3` if the gameplay quality matches that tier.
7. A player may win narrowly and receive a lower low-tier result if the tester evaluates the gameplay below `LT3`.
8. A normal low-tier test cannot directly award `HT3` or higher.
9. A regular low-tier test does not require a recording.
10. Staff may request evidence when investigating a possible rules violation, but neither participant is required to record every low-tier test.
11. A player who violates test rules may receive Restricted immediately.
12. The player may appeal a disputed low-tier evaluation.

Required stored data for normal low-tier tests remains minimal. Exact storage fields are `TBD` until implementation.

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
2. If the applicant wins `4:0` or `4:1`, the applicant receives `LT3` immediately.
3. The applicant may choose to keep `LT3` or enter the bonus HT3 skip-test queue.
4. The bonus HT3 test is played against a senior tester.
5. The bonus test also uses `First to 4`.
6. Any win against the senior tester grants `HT3` and replaces the temporary `LT3` result.
7. If the applicant loses, the existing `LT3` result remains.
8. The applicant may leave the skip-test queue and keep `LT3`.
9. The skip-test opportunity remains available until a senior tester opens and starts a matching queue.
10. A skip-test does not create an additional cooldown.
11. Completing or failing a skip-test does not create an additional cooldown.
12. A bonus skip-test does not require a recording by default.

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
- record the result when required by the implementation.

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

Confirmed opponent selection rule:

- the opponent must differ by no more than one ladder step;
- low-tier and high-tier league boundaries must still be respected.

Example:

- an `HT3` player may play against `HT3` or `LT2`;
- an `HT3` player may not use `LT3` as an opponent because `LT3` belongs to the low-tier league.

The exact relation between current tier, target tier and phase-specific opponents remains `TBD` until the high-tier phase rules are finalized.

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
- chat remains visible;
- scoreboard remains visible when the server provides one;
- the complete original recording must be available for review;
- one or both players may submit recordings;
- a hidden YouTube link may be used;
- CPVP.PRO should store links rather than large video files.

### Option B — Senior tester spectator

A senior tester spectates the match and observes the full fight.

Requirements:

- the server is agreed in advance;
- the senior tester observes the complete match;
- the senior tester records the result and notes;
- an additional recording is not required by default.

Staff may request a second participant recording when a dispute requires additional evidence.

## Recording verdicts

The exact reviewer composition is still `TBD` and must be confirmed later.

Confirmed rules:

1. A verdict should be issued within `24–72 hours`.
2. If reviewers agree, the verdict is accepted.
3. If reviewers disagree, staff resolves the case.
4. The player receives the result and a short reason.
5. Internal review notes may temporarily be stored in Discord during alpha.
6. The final verdict should be stored in the CPVP.PRO database during implementation.

## Cooldown

- A normal tier-test application can be submitted once per week.
- The cooldown begins after the verdict.
- If the tester cancels or does not appear, the cooldown is not applied.
- If the test is cancelled for a technical reason, the cooldown is not applied.
- If the player loses a completed normal test, the weekly cooldown still applies.
- Only one active application is allowed per player.
- A player may cancel the application before a tester is assigned.
- Skip-tests do not create an additional cooldown.

## High-tier progression reference

The exact phase structure for `LT2`, `HT2`, `LT1` and `HT1` will be finalized during implementation.

Current external reference material should remain separate from official CPVP.PRO rules.

## Rules still to finalize during implementation

- detailed Vanilla kit rules;
- exact phase requirements for `LT2`, `HT2`, `LT1`, `HT1`;
- exact high-tier reviewer composition;
- biome striking rules;
- cross-region and ping equalization rules;
- allowed and disallowed mods;
- anti-cheating policy details;
- appeal flow details;
- exact evidence upload format;
- exact retention period for external recording links;
- detailed Unranked permissions;
- Restricted violation mapping;
- queue implementation details.
