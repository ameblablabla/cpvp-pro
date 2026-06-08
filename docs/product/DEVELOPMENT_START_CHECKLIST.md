# CPVP.PRO development start checklist

## Read first

Before writing feature code:

1. Review [`PROJECT_OVERVIEW.md`](PROJECT_OVERVIEW.md).
2. Review [`ROADMAP.md`](ROADMAP.md).
3. Review [`INFORMATION_ARCHITECTURE.md`](INFORMATION_ARCHITECTURE.md).
4. Review the official drafts under `docs/rules/`.
5. Keep unresolved details marked `TBD` instead of inventing behavior.

## First technical decisions

- [ ] Choose frontend stack.
- [ ] Choose backend stack.
- [ ] Choose database.
- [ ] Choose hosting for application and database.
- [ ] Define local development environment.
- [ ] Define environment variables.
- [ ] Add staging deployment.
- [ ] Add migration strategy.
- [ ] Add localization strategy for Russian and English.

## First implementation milestone: learning

- [ ] Add browser-language auto-detection.
- [ ] Add navbar language switcher.
- [ ] Add Discord OAuth sign-in.
- [ ] Add basic profiles and settings.
- [ ] Add learning categories.
- [ ] Add guide pages.
- [ ] Add search and filters.
- [ ] Add progress tracking.
- [ ] Add reactions under guides.
- [ ] Add paid learning subscription tiers.
- [ ] Add subscription entitlements.
- [ ] Add top-level profile cosmetics for paid subscribers.

## Second implementation milestone: community

- [ ] Add notifications.
- [ ] Add player following with configurable notifications.
- [ ] Add Find Duel.
- [ ] Add teams, team applications and invitations.
- [ ] Add public team pages.
- [ ] Add team rating and team matches.

## Third implementation milestone: Vanilla CPVP TierList

- [ ] Add licensed Minecraft Java Edition linking through official Microsoft OAuth.
- [ ] Add Verified Player status.
- [ ] Add tier ladder and player states.
- [ ] Add regional waitlists and high-tier tickets.
- [ ] Add low-tier evaluation flow.
- [ ] Add HT3 skip-test flow.
- [ ] Add high-tier evidence review.
- [ ] Add verdict history.
- [ ] Add appeals.
- [ ] Add tester panel.

## Quality gates

- [ ] Add rate limiting.
- [ ] Add audit logging.
- [ ] Add backup strategy.
- [ ] Add file and link validation.
- [ ] Add error monitoring.
- [ ] Add performance monitoring.
- [ ] Review accessibility.
- [ ] Run closed testing.

## Deliberately postponed details

These remain `TBD` until the owner provides final rules:

- detailed Vanilla CPVP kit rules;
- final LT2, HT2, LT1 and HT1 phase details;
- final cross-region and ping-equalization details;
- final biome-striking details;
- complete allowed-mod list;
- exact punishment matrix;
- exact high-tier reviewer role naming;
- exact recording-link retention period.
