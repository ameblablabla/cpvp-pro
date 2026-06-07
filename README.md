<div align="center">
  <img src="assets/readme-banner.svg" alt="CPVP.PRO — Crystal PvP Platform" width="100%">
</div>

# CPVP.PRO

**CPVP.PRO** — будущая русскоязычная платформа для игроков Minecraft Crystal PvP. Проект объединит обучение, TierList игроков, форум и комьюнити-инструменты в одном интерфейсе.

Сейчас в репозитории находится оптимизированная временная landing page для домена [`cpvp.pro`](https://cpvp.pro/).

## Статус

> **In development** — публичная версия платформы ещё не запущена.

Подготовлены домен, landing page, документация продукта, первые desktop-макеты, Canva-исходники и полный production branding pack.

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

## Документация

### Product foundation

- [`docs/PROJECT.md`](docs/PROJECT.md)
- [`docs/ROADMAP.md`](docs/ROADMAP.md)
- [`docs/INFORMATION_ARCHITECTURE.md`](docs/INFORMATION_ARCHITECTURE.md)
- [`docs/UI_KIT.md`](docs/UI_KIT.md)
- [`docs/DESIGN.md`](docs/DESIGN.md)
- [`docs/FIGMA_STATUS.md`](docs/FIGMA_STATUS.md)
- [`docs/BRANDING_STATUS.md`](docs/BRANDING_STATUS.md)

### Product rules and content

- [`docs/ROLES_AND_MODERATION.md`](docs/ROLES_AND_MODERATION.md)
- [`docs/TIERLIST_RULES.md`](docs/TIERLIST_RULES.md)
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
│   │   ├── announcement-template.png
│   │   ├── apple-touch-icon.png
│   │   ├── favicon.ico
│   │   ├── favicon.svg
│   │   ├── logo-mark.png
│   │   ├── logo-mark.svg
│   │   ├── logo.svg
│   │   ├── og-image.png
│   │   ├── social-cover.png
│   │   └── story-template.png
│   └── readme-banner.svg
├── docs/
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

## Roadmap

- [x] Подключить домен `cpvp.pro`
- [x] Разместить и оптимизировать landing page
- [x] Добавить SEO-основу
- [x] Добавить полный branding pack
- [x] Подключить favicon pack, OG image и webmanifest
- [x] Оформить репозиторий и документацию
- [x] Подготовить desktop-макеты в Figma
- [x] Подготовить Canva-исходники
- [x] Подготовить drafts правил, FAQ и контент-планов
- [ ] Подготовить mobile-макеты
- [ ] Перейти к разработке полноценной платформы

Полная версия roadmap находится в [`docs/ROADMAP.md`](docs/ROADMAP.md).

## Лицензия

Лицензия пока не выбрана. До появления отдельного файла `LICENSE` исходный код проекта не считается открытым для свободного копирования, изменения или распространения.
