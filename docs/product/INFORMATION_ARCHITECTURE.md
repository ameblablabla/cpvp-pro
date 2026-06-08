# CPVP.PRO information architecture

## Product layers

CPVP.PRO is a bilingual Crystal PvP community platform. Learning ships first. TierList and testing follow after the learning foundation is stable. Forum is intentionally a later-stage feature.

## Public navigation

```text
/
├── learn
│   ├── guides
│   ├── mechanics
│   ├── mistakes
│   └── progress
├── players
│   └── :minecraftUsername
├── find-duel
├── teams
│   └── :teamSlug
├── rules
├── faq
├── tiers                 # later release
│   ├── vanilla-cpvp
│   ├── history
│   └── coming-soon
└── forum                 # later release
    ├── categories
    ├── topics
    └── :topicSlug
```

## Account navigation

```text
/account
├── profile
├── minecraft-link
├── learning
├── subscriptions
├── notifications
├── privacy
└── settings
```

## Moderation navigation

```text
/moderation
├── reports
├── appeals
├── users
├── punishments
└── audit-log
```

## Tester panel

```text
/tester
├── waitlists
├── low-tier-tests
├── high-tier-tickets
├── recordings
├── verdicts
├── complaints
└── instructions
```

## First public release

Required:

1. Home.
2. Learning catalog.
3. Guide pages.
4. Search and filters.
5. Learning progress.
6. Discord OAuth sign-in.
7. Basic player profiles.
8. Account settings.
9. Notifications.
10. Russian-English localization.
11. Browser-language auto-detection.
12. Navbar language switcher.
13. Paid learning subscription tiers.

## Later releases

### Community layer

- Find Duel;
- teams;
- following players;
- configurable notifications;
- Discord and Telegram integration.

### Vanilla CPVP TierList

- public ladder;
- Minecraft account linking;
- applications;
- queues;
- tester panel;
- high-tier review;
- appeals.

### Forum

- categories;
- topics;
- replies;
- reactions;
- reports;
- moderation.
