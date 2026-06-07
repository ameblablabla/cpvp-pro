# CPVP.PRO testing requirements snapshot

## Category

```text
Vanilla CPVP
```

Vanilla CPVP is the first and only confirmed category for the initial version.

## Ladder

From lowest to highest:

```text
LT5 < HT5 < LT4 < HT4 < LT3 < HT3 < LT2 < HT2 < LT1 < HT1
```

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

## Player states

### Unranked

Display:

```text
Unranked
```

Confirmed access:

- forum participation;
- Find Duel;
- teams;
- following players;
- guide comments.

Other restrictions remain `TBD`.

### Retired

Confirmed:

- player enables Retired voluntarily;
- reason required;
- may be enabled immediately after receiving a tier;
- minimum period: three months;
- no tests while Retired;
- retest required after leaving Retired;
- public Retired badge;
- display uses `R` prefix.

Examples:

```text
RLT3
RHT5
RHT3
```

### Inactive

Applies to `HT3+` only.

Confirmed:

- at least one official test per month or Retired status required;
- frequent reminders before deadline;
- missed deadline sets `Inactive`;
- tier drops to `LT3` from any high-tier rank.

### Restricted

Escalation:

```text
First Restricted: 1 month
Second Restricted: 90 days
Third Restricted: permanent project ban
```

Confirmed:

- tiers reset;
- previous tier history remains visible;
- Restricted badge remains permanently visible in profile history;
- appeal allowed;
- after temporary Restricted ends, player returns as `Unranked`.

## Match format

Default format:

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

Confirmed:

- players continue until one reaches four wins;
- technical replays are allowed;
- tester responsible for the match decides replay requirement;
- ping should be recorded where practical;
- professional cross-region and ping-equalization rules should be used;
- biome striking may be used for high-tier tests.

Exact cross-region, ping-equalization and biome-striking rules remain `TBD` and should be adapted from the external reference.

## Applications and queues

Required application fields:

- server region;
- Minecraft username used for testing;
- preferred time;
- preferred server.

Confirmed:

- false information results in denied testing;
- only one active application per player;
- player may cancel before tester assignment.

### Low-tier waitlist flow

1. Player submits an application.
2. Player is added to a waitlist channel.
3. Tester of the requested region opens a queue when available.
4. Players are pinged.
5. Player joins queue and completes test.

### High-tier flow

Players with `HT3+` use a high-ticket flow instead of the low-tier waitlist.

## Cooldown

Confirmed:

- normal tier-test application: once per week;
- cooldown begins after verdict;
- no cooldown if tester cancels or does not appear;
- no cooldown if match is cancelled for technical reasons;
- losing a completed normal test still creates cooldown;
- skip-tests do not create additional cooldown;
- completing or failing skip-test does not create additional cooldown.

## Low-tier tests

Confirmed:

- one match against regular tester;
- `First to 4`;
- tester and applicant agree on server;
- tester evaluates approximate tier from gameplay;
- tester may assign any low-tier result from `LT5` to `LT3`;
- `LT5` is minimum tier;
- score does not automatically determine result;
- player may lose and still receive `LT3` if gameplay quality matches;
- player may win narrowly and receive lower rank if gameplay is weaker;
- no mandatory recording;
- staff may request evidence during a rules-violation investigation;
- rule violation during test may trigger immediate Restricted;
- low-tier verdict may be appealed.

## HT3 skip-test

Qualification:

```text
4:0
4:1
```

Confirmed:

- qualifying player receives `LT3` immediately;
- player may keep `LT3` or enter bonus queue;
- bonus opponent is a senior tester;
- bonus match uses `First to 4`;
- any win grants `HT3` and replaces `LT3`;
- loss keeps `LT3`;
- player may leave queue and keep `LT3`;
- opportunity lasts until senior tester opens and starts a matching queue;
- no mandatory recording;
- no additional cooldown.

## High-tier tests

Confirmed:

- begin at `HT3`;
- applicant plays a real ranked player;
- opponent differs by no more than one ladder step;
- low/high league boundary must be respected;
- `HT3` may play `HT3` or `LT2`;
- `HT3` may not use `LT3`;
- server agreed by both players;
- one `First to 4` match except T1 phase rules.

Exact relation between current rank, target rank and phase-specific opponents remains `TBD`.

## High-tier evidence

Use one of two methods.

### Full recording

Required:

- starts before joining server;
- agreed IP visible during direct connect;
- Minecraft username visible;
- full match recorded;
- uncut recording;
- hotbar visible;
- normal HUD visible;
- chat visible;
- scoreboard visible when available;
- original full recording available;
- one or both players may submit;
- hidden YouTube links allowed;
- store links rather than large video files;
- staff may request second-player recording in disputes.

Voice and Discord-screen recording are not required.

### Senior tester spectator

Required:

- agreed server;
- full match observation;
- result and notes recorded;
- additional recording not required by default.

## High-tier verdict

Confirmed:

- target verdict time: `24–72 hours`;
- if reviewers agree, verdict accepted;
- if reviewers disagree, staff resolves;
- no third reviewer required by default;
- player receives result and short reason;
- internal notes may temporarily live in Discord during alpha;
- final verdict should be stored in the site database.

Exact reviewer-role composition remains `TBD`.
