# CPVP.PRO product requirements / Требования продукта

## Positioning / Позиционирование

RU: CPVP.PRO — русскоязычная и англоязычная платформа и постоянно расширяющееся комьюнити игроков Crystal PvP. TierList и тиртесты важны, но не являются единственной функцией проекта.

EN: CPVP.PRO is a bilingual Russian-English platform and an expanding Crystal PvP community. TierList and tier testing are important, but they are not the whole product.

## First-priority sections / Приоритетные разделы

Confirmed first-priority sections:

- Home / Главная;
- Player profiles / Профили игроков;
- Rules / Правила;
- FAQ;
- Learning / Обучение;
- Moderation panel / Модераторская панель;
- Account settings / Настройки аккаунта;
- Notifications / Уведомления.

Additional confirmed direction:

- Learning is an early priority because it was the original product idea.
- Forum is expected to be one of the final stages.
- A separate Community page is not required.
- Community functionality should be distributed across profiles, teams, Find Duel, forum and external channels.
- All public product surfaces should support Russian and English.

TierList and tier-test applications are core features. Whether they must be included in the very first release package remains `TBD` for final confirmation.

## First category / Первая категория

```text
Vanilla CPVP
```

Confirmed:

- Vanilla CPVP is one overall category.
- Players build kits according to the Vanilla CPVP ruleset.
- Detailed kit rules will be added later.
- Future categories may be displayed as coming soon.
- Dynamic category creation through an admin panel is not required for the initial version.

## Community features / Комьюнити-функции

Confirmed:

- Discord is the main external community channel.
- Telegram is required as an announcement channel.
- On-site news are probably not required initially.
- Find Duel is required.
- Player teams are required.
- Guide comments are required.
- Likes or reactions are required.
- On-site direct messages are not required because Discord is sufficient.

## Documentation principles / Принципы документации

Public documents required:

- platform rules;
- forum rules;
- Vanilla kit rules;
- tier-test rules;
- cheating policy;
- mod/client rules;
- appeals;
- privacy policy;
- terms of use;
- FAQ.

Confirmed:

- public rules should be clear and concise;
- abuse-sensitive internal details should remain hidden;
- internal tester instructions should live in the tester panel on the website;
- the GitHub repository may remain public.

## Target documentation structure / Целевая структура документации

```text
docs/
├── product/
├── rules/
├── operations/
├── design/
├── content/
└── references/
```

Confirmed:

- old duplicate files should be removed after migration;
- README should remain attractive and functional;
- migration strategy (`main` or review branch) remains `TBD`.
