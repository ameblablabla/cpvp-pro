# CPVP.PRO UI kit specification

## Назначение

Этот документ фиксирует первый набор компонентов будущего интерфейса. Он нужен до начала frontend-разработки, чтобы страницы собирались из одинаковых элементов и сохраняли единый визуальный язык.

## Tokens

### Цвета

| Token | Значение | Использование |
|---|---|---|
| `--bg` | `#05070D` | основной фон |
| `--surface` | `#0D111E` | карточки и панели |
| `--surface-muted` | `#141A2B` | вторичный фон |
| `--line` | `rgba(150,180,255,.15)` | границы |
| `--text` | `#EEF4FF` | основной текст |
| `--muted` | `#9AA7BD` | вторичный текст |
| `--blue` | `#72D7FF` | основной акцент |
| `--violet` | `#9B6CFF` | дополнительный акцент |
| `--green` | `#94FFCF` | активный статус |
| `--danger` | `#FF7C92` | ошибки и предупреждения |

### Радиусы

| Token | Значение |
|---|---|
| `--radius-sm` | `12px` |
| `--radius-md` | `18px` |
| `--radius-lg` | `26px` |
| `--radius-pill` | `999px` |

### Отступы

Основная шкала: `4`, `8`, `12`, `16`, `24`, `32`, `48`, `64` пикселей.

## Базовые компоненты

### Navigation

- Desktop navbar.
- Mobile top bar.
- Mobile menu drawer.
- Breadcrumbs.
- Tabs.

### Buttons

- Primary action.
- Secondary action.
- Ghost action.
- Danger action.
- Icon button.

Каждая кнопка должна иметь состояния `default`, `hover`, `focus-visible`, `disabled`, `loading`.

### Cards

- Feature card.
- Player card.
- Tier card.
- Guide card.
- Forum topic card.
- Profile stat card.
- Moderation report card.

### Forms

- Text input.
- Search input.
- Textarea.
- Select.
- Checkbox.
- Radio.
- Switch.
- Validation message.

### Feedback

- Status badge.
- Tier badge.
- Toast.
- Empty state.
- Loading skeleton.
- Inline alert.
- Confirmation modal.

## Page templates

Нужны готовые шаблоны для:

1. Главной страницы.
2. Списка гайдов.
3. Страницы гайда.
4. TierList.
5. Публичного профиля игрока.
6. Категории форума.
7. Темы форума.
8. Настроек профиля.
9. Очереди модерации.

## Правила доступности

- У интерактивных элементов должен быть заметный `focus-visible`.
- Цвет не должен быть единственным способом передачи статуса.
- Для иконок без текста нужен `aria-label`.
- Контраст текста должен оставаться читаемым на тёмном фоне.
- Анимации должны учитывать `prefers-reduced-motion`.
