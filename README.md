<div align="center">
  <img src="assets/readme-banner.svg" alt="CPVP.PRO — Crystal PvP Platform" width="100%">
</div>

# CPVP.PRO

**CPVP.PRO** — развивающаяся русскоязычная и англоязычная платформа для игроков Minecraft Crystal PvP. Проект объединит обучение, профили игроков, Vanilla CPVP TierList, правила, уведомления, Find Duel, команды и другие комьюнити-инструменты.

CPVP.PRO не ограничивается тиртестами: tier testing является важной частью платформы, но не единственным назначением сайта.

Сейчас в репозитории находится оптимизированная временная landing page для домена [`cpvp.pro`](https://cpvp.pro/).

## Статус

> **In development** — публичная версия платформы ещё не запущена.

Подготовлены домен, landing page, production branding pack, документация продукта, первые desktop-макеты и подробные requirements snapshots перед началом разработки.

## Главный источник требований

Ответы из большого продуктового опроса сохранены в [`docs/snapshots/README.md`](docs/snapshots/README.md).

В snapshots разделены:

- позиционирование продукта и двуязычность;
- Vanilla CPVP ladder;
- low-tier, skip-test и high-tier правила;
- Unranked, Retired, Inactive и Restricted состояния;
- Discord OAuth и безопасная Minecraft-привязка;
- публичные профили;
- tester и senior tester роли;
- комьюнити-функции;
- незакрытые вопросы `TBD` для короткого уточнения позже;
- внешние референсы, которые пока не считаются официальными правилами CPVP.PRO.

Пока snapshots являются временным источником истины. После уточнения оставшихся `TBD` документация будет перенесена в финальную структуру без дублей.

## Зафиксированная Vanilla CPVP система

Первая competitive-категория:

```text
Vanilla CPVP
```

Полная ladder-шкала:

```text
LT5 < HT5 < LT4 < HT4 < LT3 < HT3 < LT2 < HT2 < LT1 < HT1
```

Основные подтверждённые решения:

- low-tier и high-tier лиги разделены;
- обычные тестеры проводят low-tier тесты и могут выдать максимум `LT3`;
- опытный тестер оценивает примерный тир игрока по реальной игре;
- `4:0` или `4:1` против обычного тестера дают шанс на HT3 skip-test;
- qualifying игрок сразу получает `LT3`, а затем может заменить его на `HT3`;
- HT3 skip-test играется против senior tester;
- high-tier тесты играются против ranked players близкого уровня;
- стандартный формат матчей: `First to 4`;
- normal high-tier тест требует полной записи или senior tester spectator verification;
- normal tier-test заявку можно подавать раз в неделю;
- cooldown начинается после verdict;
- testing доступен только для Minecraft Java Edition на ПК или ноутбуке;
- мобильная версия сайта предназначена для просмотра, заявок и управления профилем.

Подробности:

- [`docs/VANILLA_TESTING_RULES.md`](docs/VANILLA_TESTING_RULES.md)
- [`docs/TIERLIST_RULES.md`](docs/TIERLIST_RULES.md)
- [`docs/snapshots/TESTING_REQUIREMENTS.md`](docs/snapshots/TESTING_REQUIREMENTS.md)

## Аккаунты

Tier-test заявку сможет подать только авторизованный пользователь с подтверждённым лицензированным Minecraft Java Edition аккаунтом.

Подтверждено:

- вход на сайт через Discord OAuth;
- Discord-аккаунт обязателен;
- Minecraft-привязка предпочтительно через официальный Microsoft OAuth;
- один CPVP.PRO аккаунт связывается только с одним Minecraft UUID;
- один Minecraft UUID связывается только с одним CPVP.PRO аккаунтом;
- свободная смена или self-service unlink не требуются;
- CPVP.PRO не должен запрашивать или хранить Microsoft-пароль, Minecraft-пароль или session token.

Подробности:

- [`docs/ACCOUNT_LINKING.md`](docs/ACCOUNT_LINKING.md)
- [`docs/snapshots/ACCOUNT_PROFILE_REQUIREMENTS.md`](docs/snapshots/ACCOUNT_PROFILE_REQUIREMENTS.md)

## Дизайн

### Figma

Основной файл:

[`CPVP.PRO — UI Kit and Product Layouts`](https://www.figma.com/design/7VjJ1bfnfWLSnxIJOTHko9/CPVP.PRO-%E2%80%94-UI-Kit-and-Product-Layouts?node-id=0-1&p=f)

Уже готовы:

- cover;
- foundations;
- UI-kit;
- desktop home;
- desktop learning;
- desktop TierList;
- desktop forum.

Оставшиеся mobile-макеты и дополнительные desktop-экраны будут добавлены позже.

### Canva

Редактируемые исходники:

- [logo and wordmark](https://www.canva.com/d/i0h_0fPMxTsPaFN);
- [wide social cover](https://www.canva.com/d/4z_sqetriJFXBbc);
- [square announcement post](https://www.canva.com/d/gmSwOh1DreTnhJN);
- [vertical story template](https://www.canva.com/d/q3k1ftX70akt_El).

Production branding pack полностью загружен в `assets/branding/`.

## Документация

### Временный источник истины перед реструктуризацией

- [`docs/snapshots/README.md`](docs/snapshots/README.md)
- [`docs/snapshots/TBD_DECISIONS.md`](docs/snapshots/TBD_DECISIONS.md)
- [`docs/references/EXTERNAL_TIER_SYSTEM_REFERENCE.md`](docs/references/EXTERNAL_TIER_SYSTEM_REFERENCE.md)

### Основные текущие документы

- [`docs/PROJECT.md`](docs/PROJECT.md)
- [`docs/ROADMAP.md`](docs/ROADMAP.md)
- [`docs/DEVELOPMENT_START_CHECKLIST.md`](docs/DEVELOPMENT_START_CHECKLIST.md)
- [`docs/VANILLA_TESTING_RULES.md`](docs/VANILLA_TESTING_RULES.md)
- [`docs/TIERLIST_RULES.md`](docs/TIERLIST_RULES.md)
- [`docs/ACCOUNT_LINKING.md`](docs/ACCOUNT_LINKING.md)
- [`docs/ROLES_AND_MODERATION.md`](docs/ROLES_AND_MODERATION.md)
- [`docs/FAQ.md`](docs/FAQ.md)

## Landing page

Текущая страница намеренно сделана лёгкой:

- без JavaScript;
- без фреймворков;
- без внешних шрифтов;
- без внешнего CSS;
- с адаптивной мобильной версией;
- с `prefers-reduced-motion`;
- с SVG favicon и ICO fallback;
- с Apple touch icon;
- с `site.webmanifest`;
- с canonical URL;
- с Open Graph image;
- с Twitter image;
- с `robots.txt` и `sitemap.xml`.

## Локальный запуск

```bash
python -m http.server 8080
```

Страница будет доступна по адресу `http://localhost:8080`.

## Что делать при начале разработки

1. Открыть [`docs/DEVELOPMENT_START_CHECKLIST.md`](docs/DEVELOPMENT_START_CHECKLIST.md).
2. Перечитать snapshots.
3. Закрыть оставшиеся `TBD` короткими вопросами.
4. Перенести документы в финальную структуру без дублей.
5. Выбрать frontend, backend и базу данных.
6. Создать первую architecture branch.
7. Начать с аккаунтов, профилей и безопасной Minecraft Java Edition привязки.

## Roadmap

Полная версия roadmap находится в [`docs/ROADMAP.md`](docs/ROADMAP.md).

## Лицензия

Лицензия пока не выбрана. До появления отдельного файла `LICENSE` исходный код проекта не считается открытым для свободного копирования, изменения или распространения.
