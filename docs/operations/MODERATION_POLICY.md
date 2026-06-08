# CPVP.PRO moderation policy

## Principles

- Decisions must be understandable and reviewable.
- Similar cases should be handled consistently.
- Important actions must be logged.
- Users should see the reason for restrictions.
- Appeals are reviewed separately from the original decision.

## Case types

```text
forum_report
profile_report
tester_complaint
tier_verdict_appeal
punishment_appeal
account_link_review
```

## Statuses

```text
new
in_review
resolved
rejected
```

## Base workflow

1. Case enters a queue.
2. Moderator or staff reviews available evidence.
3. Additional information may be requested.
4. Decision is recorded with a short reason.
5. User receives a notification.
6. Appeal remains available where allowed.

## Available actions

Depending on severity:

- warning;
- mute;
- content hiding;
- forum restriction;
- testing restriction;
- Restricted status;
- temporary account ban;
- permanent project ban.

## Restricted history

- punishment badge remains visible in profile history;
- hover state shows details;
- previous tier history remains visible;
- first Restricted lasts one month;
- second Restricted lasts ninety days;
- third Restricted is a permanent project ban.

## Tester oversight

- tester complaints are supported;
- tester match history is stored;
- tester status may be `active`, `inactive` or `suspended`;
- staff may remove tester permissions for poor decisions or rule violations.

## Internal notes

- internal notes may remain in Discord;
- final verdicts and platform actions must be stored in the CPVP.PRO database;
- audit-log access is limited to authorized roles.
