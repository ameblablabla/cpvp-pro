<div align="center">
  <img src="assets/readme-banner.svg" alt="CPVP.PRO — Crystal PvP Platform" width="100%">
</div>

# CPVP.PRO

**CPVP.PRO** — развивающаяся русскоязычная платформа для игроков Minecraft Crystal PvP. Проект объединит обучение, профили игроков, Vanilla TierList, форум, новости и комьюнити-инструменты в одном интерфейсе.

CPVP.PRO не ограничивается тиртестами: tier testing является важной частью платформы, но не единственным назначением сайта.

Сейчас в репозитории находится оптимизированная временная landing page для домена [`cpvp.pro`](https://cpvp.pro/).

## Статус

> **In development** — публичная версия платформы ещё не запущена.

Подготовлены домен, landing page, документация продукта, первые desktop-макеты, Canva-исходники, production branding pack и спецификация Vanilla tier-testing системы.

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

Оставшиеся mobile-макеты и дополнительные desktop-экраны будут добавлены после сброса лимита Figma Starter MCP.

### Canva

Редактируемые исходники:

- [logo and wordmark](https://www.canva.com/d/i0h_0fPMxTsPaFN);
- [wide social cover](https://www.canva.com/d/4z_sqetriJFXBbc);
- [square announcement post](https://www.canva.com/d/gmSwOh1DreTnhJN);
- [vertical story template](https://www.canva.com/d/q3k1ftX70akt_El).

Production branding pack полностью загружен в `assets/branding/`. На landing page подключены SVG favicon, ICO fallback, Apple touch icon, Open Graph image, Twitter image и `site.webmanifest`.

## Зафиксированная Vanilla-система

Первая competitive-категория:

```text
Vanilla
```

Полная ladder-шкала:

```text
LT5 < HT5 < LT4 < HT4 < LT3 < HT3 < LT2 < HT2 < LT1 < HT1
```

Основные решения:

- low-tier и high-tier лиги разделены;
- обычные тестеры проводят low-tier тесты и могут выдать максимум `LT3`;
- опытный тестер должен по игре оценить примерный тир заявителя;
- `4:0` или `4:1` против обычного тестера дают шанс на HT3 skip-test;
- HT3 skip-test играется против senior tester;
- high-tier тесты играются против реальных ranked players близкого уровня;
- формат матчей: `First to 4`;
- high-tier тесты требуют полной записи или senior tester spectator verification;
- записи смотрят минимум два senior tester;
- при разногласии решение принимает staff;
- tier-test заявку можно подавать раз в неделю;
- тестирование доступно только для Minecraft Java Edition на ПК или ноутбуке;
- мобильная версия сайта нужна для удобного просмотра и управления заявками.

Подробности:

- [`docs/VANILLA_TESTING_RULES.md`](docs/VANILLA_TESTING_RULES.md)
- [`docs/TIERLIST_RULES.md`](docs/TIERLIST_RULES.md)
- [`docs/ROLES_AND_MODERATION.md`](docs/ROLES_AND_MODERATION.md)

## Безопасная привязка Minecraft-аккаунта

Tier-test заявку сможет подать только авторизованный пользователь с привязанным и подтверждённым лицензированным Minecraft Java Edition аккаунтом.

CPVP.PRO не должен запрашивать Microsoft-пароль, Minecraft-пароль или session token. Привязка нужна для подтверждения личности игрока и ответственности за профиль, а не для получения доступа к аккаунту.

Требования и безопасные варианты реализации:

- [`docs/ACCOUNT_LINKING.md`](docs/ACCOUNT_LINKING.md)

## Документация

### Product foundation

- [`docs/PROJECT.md`](docs/PROJECT.md)
- [`docs/ROADMAP.md`](docs/ROADMAP.md)
- [`docs/DEVELOPMENT_START_CHECKLIST.md`](docs/DEVELOPMENT_START_CHECKLIST.md)
- [`docs/INFORMATION_ARCHITECTURE.md`](docs/INFORMATION_ARCHITECTURE.md)
- [`docs/UI_KIT.md`](docs/UI_KIT.md)
- [`docs/DESIGN.md`](docs/DESIGN.md)
- [`docs/FIGMA_STATUS.md`](docs/FIGMA_STATUS.md)
- [`docs/BRANDING_STATUS.md`](docs/BRANDING_STATUS.md)

### Product rules and content

- [`docs/VANILLA_TESTING_RULES.md`](docs/VANILLA_TESTING_RULES.md)
- [`docs/TIERLIST_RULES.md`](docs/TIERLIST_RULES.md)
- [`docs/ACCOUNT_LINKING.md`](docs/ACCOUNT_LINKING.md)
- [`docs/ROLES_AND_MODERATION.md`](docs/ROLES_AND_MODERATION.md)
- [`docs/PLATFORM_RULES.md`](docs/PLATFORM_RULES.md)
- [`docs/FORUM_RULES.md`](docs/FORUM_RULES.md)
- [`docs/MODERATION_POLICY.md`](docs/MODERATION_POLICY.md)
- [`docs/FAQ.md`](docs/FAQ.md)
- [`docs/LEARNING_CONTENT_PLAN.md`](docs/LEARNING_CONTENT_PLAN.md)
- [`docs/COMMUNITY_PLAN.md`](docs/COMMUNITY_PLAN.md)
- [`docs/RELEASE_CHECKLIST.md`](docs/RELEASE_CHECKLIST.md)
- [`CONTRIBUTING.md`](CONTRIBUTING.md)

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

## Автоматическая проверка

Workflow `.github/workflows/validate-static-site.yml` запускается для `main` и Pull Request. Он проверяет обязательные файлы, домен, SEO-основу, отсутствие JavaScript, отсутствие внешнего CSS и отсутствие Google Fonts.

## Структура репозитория

```text
cpvp-pro/
├── .github/
│   ├── ISSUE_TEMPLATE/
│   ├── workflows/
│   ├── CODEOWNERS
│   └── PULL_REQUEST_TEMPLATE.md
├── assets/
│   ├── branding/
│   └── readme-banner.svg
├── docs/
│   ├── ACCOUNT_LINKING.md
│   ├── DEVELOPMENT_START_CHECKLIST.md
│   ├── VANILLA_TESTING_RULES.md
│   └── ...
├── .editorconfig
├── .gitignore
├── .nojekyll
├── 404.html
├── CNAME
├── CONTRIBUTING.md
├── README.md
├── index.html
├── robots.txt
├── sitemap.xml
└── site.webmanifest
```

## Локальный запуск

```bash
python -m http.server 8080
```

Страница будет доступна по адресу `http://localhost:8080`.

## Что делать при начале разработки

Перед написанием feature-кода:

1. Открыть [`docs/DEVELOPMENT_START_CHECKLIST.md`](docs/DEVELOPMENT_START_CHECKLIST.md).
2. Перечитать [`docs/VANILLA_TESTING_RULES.md`](docs/VANILLA_TESTING_RULES.md).
3. Перечитать [`docs/ACCOUNT_LINKING.md`](docs/ACCOUNT_LINKING.md).
4. Выбрать frontend, backend и базу данных.
5. Создать первую architecture branch.
6. Начать с аккаунтов, профилей и безопасной привязки Minecraft Java Edition аккаунта.

## Roadmap

- [x] Подключить домен `cpvp.pro`
- [x] Разместить и оптимизировать landing page
- [x] Добавить SEO-основу
- [x] Добавить полный branding pack
- [x] Оформить репозиторий и документацию
- [x] Подготовить desktop-макеты в Figma
- [x] Подготовить Canva-исходники
- [x] Зафиксировать Vanilla testing model
- [x] Зафиксировать safe Minecraft account-linking requirements
- [x] Подготовить development-start checklist
- [ ] Подготовить mobile-макеты
- [ ] Выбрать стек
- [ ] Начать разработку полноценной платформы

Полная версия roadmap находится в [`docs/ROADMAP.md`](docs/ROADMAP.md).

## Лицензия

Лицензия пока не выбрана. До появления отдельного файла `LICENSE` исходный код проекта не считается открытым для свободного копирования, изменения или распространения.
