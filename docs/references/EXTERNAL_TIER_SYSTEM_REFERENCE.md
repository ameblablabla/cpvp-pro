# External tier system reference

> Reference only. Not an official CPVP.PRO ruleset.

This file preserves external ideas supplied during planning so they are not lost. They must not be treated as official CPVP.PRO rules until explicitly confirmed and adapted.

## Reference topics

- phased testing for `HT3`, `LT2`, `HT2`, `LT1`, `HT1`;
- title-holder style `HT1` logic;
- missing-opponent replacement logic;
- cross-region testing;
- ping equalization;
- tick-range handling;
- biome striking;
- cheating restrictions;
- client and mod rules;
- failed-test handling;
- test reopening in edge cases.

## Phase references

### HT3

- evaluation phase;
- qualification through strong regular-tester result;
- match against HT3 opponent.

### LT2 / HT2

- matches against nearby-tier opponents;
- target-tier score requirements.

### LT1

- nearby-tier matches;
- target-tier performance requirements;
- minimum-round expectations.

### HT1

- lower high-tier opponents;
- HT2 opponents;
- current-tier opponents;
- possible final match against current HT1 title holder.

## Missing opponents reference

Possible fallback idea:

```text
1 missing opponent = 2 lower-tier opponents
```

## Ping equalization reference

External reference ideas:

- cross-region testing when local opponents are unavailable;
- equalized ping within a limited difference;
- same tick-range requirement;
- tick range considered in 50 ms bands.

Exact CPVP.PRO rules remain `TBD`.

## Biome striking reference

Potential high-tier feature:

- predefined biome pool;
- players remove options until one remains;
- first-strike order alternates between matches;
- optional when both players agree on a location.

Exact CPVP.PRO implementation remains `TBD`.

## Client and mod reference

External examples that may be provisionally allowed after staff review:

- Marlow's Crystal Optimizer;
- Hero's Anchor Optimizer;
- Hero's Elytra Optimizer;
- Totem Counter.

External prohibited categories include automation, unfair information, movement irregularities, reach changes, ESP-like tools and harmful latency manipulation.

## Important note

This document exists only to preserve research input. Official player-facing rules must be written separately under `docs/rules/` after confirmation.
