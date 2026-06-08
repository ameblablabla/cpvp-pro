# CPVP.PRO Vanilla CPVP testing rules

> Official draft. Detailed kit restrictions and some advanced high-tier phase details remain `TBD` until implementation.

## 1. Scope

The first competitive category is:

```text
Vanilla CPVP
```

- Minecraft Java Edition only.
- Gameplay on PC or laptop only.
- Mobile site is for profiles, learning, rules, applications, notifications and community convenience.
- Players assemble kits according to the Vanilla CPVP kit rules.

## 2. Ladder

From lowest to highest:

```text
LT5 < HT5 < LT4 < HT4 < LT3 < HT3 < LT2 < HT2 < LT1 < HT1
```

### Low-tier league

```text
LT5
HT5
LT4
HT4
LT3
```

### High-tier league

```text
HT3
LT2
HT2
LT1
HT1
```

Low-tier and high-tier players should be visually distinguished in the interface.

## 3. Player ranking states

### Unranked

A player may exist without a tier. The profile shows:

```text
Unranked
```

Confirmed Unranked access:

- view learning materials;
- view TierList;
- view player profiles;
- view rules and FAQ;
- submit a tier-test application.

Other Unranked permissions remain restricted until explicitly enabled.

### Retired

A ranked player may voluntarily freeze the current tier.

Rules:

- reason required;
- may be enabled immediately after receiving a tier;
- minimum period: three months;
- Retired players cannot participate in tier tests;
- leaving Retired requires a retest;
- public badge required;
- tier display uses the `R` prefix.

Examples:

```text
RLT3
RHT5
RHT3
```

### Inactive

Applies only to `HT3+` players.

Rules:

- complete at least one official test per month or enter Retired;
- send frequent reminders before deadline;
- missing deadline sets `Inactive`;
- tier drops to `LT3` regardless of previous high-tier rank.

### Restricted

Restricted is a disciplinary state.

Escalation:

```text
First Restricted: 1 month
Second Restricted: 90 days
Third Restricted: permanent project ban
```

Rules:

- tiers reset;
- previous tier history remains visible;
- Restricted badge remains permanently visible in profile history;
- badge details appear on hover;
- appeal allowed;
- after temporary Restricted ends, player returns as `Unranked`.

## 4. Match format

Default official format:

```text
First to 4
```

Possible final scores:

```text
4:0
4:1
4:2
4:3
```

Rules:

- play until one participant reaches four wins;
- technical replay is allowed;
- tester responsible for the match decides whether replay is required;
- ping should be recorded where practical;
- cross-region, ping equalization and biome striking rules are adapted from the external reference and remain `TBD` until final review.

## 5. Applications and queues

A tier-test application requires:

- authenticated CPVP.PRO account;
- verified licensed Minecraft Java Edition account;
- one active application maximum;
- server region;
- Minecraft username used for testing;
- preferred time;
- preferred server.

False information results in denied testing.

### Low-tier waitlist

1. Player submits application.
2. Player enters a waitlist channel.
3. Tester of the requested region opens a queue when available.
4. Waitlisted players are pinged.
5. Player joins and completes the test.

### High-tier ticket

Players at `HT3+` use a high-ticket flow instead of the low-tier waitlist.

## 6. Cooldown

- normal application: once per week;
- cooldown begins after verdict;
- no cooldown if tester cancels, does not appear or test is cancelled for technical reasons;
- losing a completed normal test still creates cooldown;
- player may cancel before tester assignment;
- skip-tests do not create additional cooldown;
- completing or failing a skip-test does not create additional cooldown.

## 7. Low-tier evaluation

A regular tester evaluates actual gameplay and estimates the player's approximate tier.

Rules:

- one `First to 4` match against a regular tester;
- tester and player agree on server;
- tester may assign any result from `LT5` to `LT3`;
- `LT5` is minimum tier;
- score does not automatically determine low-tier result;
- player may lose and still receive `LT3` if gameplay quality matches;
- player may win narrowly and receive a lower tier if gameplay is weaker;
- no mandatory recording;
- staff may request evidence during a rules-violation investigation;
- rule violations during test may trigger immediate Restricted;
- disputed low-tier verdict may be appealed.

## 8. Bonus HT3 skip-test

Qualification against a regular tester:

```text
4:0
4:1
```

Rules:

- qualifying player receives `LT3` immediately;
- player may keep `LT3` or enter bonus queue;
- bonus match is against a senior tester;
- bonus match uses `First to 4`;
- any win upgrades the player from `LT3` to `HT3`;
- loss keeps `LT3`;
- player may leave queue and keep `LT3`;
- opportunity remains until a senior tester opens and starts a matching queue;
- no mandatory recording by default;
- no additional cooldown.

## 9. High-tier tests

For `HT3+`:

- applicant plays a real ranked player;
- opponent differs by no more than one ladder step;
- low-tier/high-tier boundary must be respected;
- `HT3` may play `HT3` or `LT2`;
- `HT3` may not use `LT3`;
- server is agreed by both players;
- one `First to 4` match is standard except T1 phase rules.

### Advanced phase draft

The external multi-phase system for `LT2`, `HT2`, `LT1` and `HT1` is accepted as the working draft. Exact wording remains `TBD` until final owner review.

### HT1 draft

Use one active HT1 title holder for now. The final title-holder model may be revisited later.

## 10. High-tier evidence

Use one of two methods.

### Full recording

Requirements:

- recording starts before joining the agreed server;
- agreed IP is visible during direct connect;
- Minecraft username is visible;
- full match is recorded;
- no cuts;
- hotbar visible;
- normal HUD visible;
- chat visible;
- scoreboard visible when available;
- original full recording available;
- one or both players may submit;
- hidden YouTube link allowed;
- store links rather than large video files;
- staff may request second-player recording in disputes.

Voice and Discord-screen recording are not required.

### Senior tester spectator

Requirements:

- agreed server;
- full-match observation;
- result and notes recorded;
- additional recording not required by default.

## 11. High-tier verdict

- full recording is reviewed by two testers;
- if both agree, tier is confirmed;
- if they disagree, staff resolves the case;
- target verdict time: `24–72 hours`;
- player receives final result and short reason;
- internal notes may remain in Discord;
- final verdict is always stored in the CPVP.PRO database.

## 12. Still TBD

- detailed Vanilla CPVP kit rules;
- final wording for LT2, HT2, LT1 and HT1 phases;
- final cross-region rules;
- final ping-equalization rules;
- final biome-striking rules;
- complete allowed-mod list;
- exact punishment matrix;
- recording-link retention period.
