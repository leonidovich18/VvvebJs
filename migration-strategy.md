# Стратегія міграції з Bootstrap на Tailwind CSS

## Підготовка

1. ✅ Встановлено Tailwind CSS та необхідні залежності
2. ✅ Створено файл конфігурації Tailwind
3. ✅ Оновлено gulpfile.js для підтримки Tailwind

## Етапи міграції

### Етап 1: Оновлення структури проєкту

1. ✅ Створено основний файл tailwind.scss
2. ✅ Підключено Tailwind CSS в editor.html
3. ✅ Компіляція та тестування інтеграції Tailwind CSS
4. ✅ Створено компатибельні міксини для Bootstrap
5. ✅ Додано утилітарні класи для сумісності з Bootstrap

### Етап 2: Міграція компонентів

1. ✅ Визначено найбільш використовувані Bootstrap-компоненти
2. ✅ Створено еквівалентні компоненти з використанням Tailwind CSS
3. ✅ Розпочато поступову заміну компонентів Bootstrap на Tailwind
   - ✅ Верхня панель (top-panel)
   - ✅ Ліва панель (left-panel)
   - ✅ Система темної теми
   - ⬜ Права панель (right-panel)
   - ⬜ Модальні вікна
   - ⬜ Кнопки та форми
4. ⬜ Тестувати кожен компонент окремо

### Етап 3: Міграція сіткової системи

1. ⬜ Визначити місця використання сіткової системи Bootstrap
2. ⬜ Замінити на сіткову систему Tailwind CSS (flex/grid)
3. ⬜ Тестувати адаптивність на різних пристроях

### Етап 4: Міграція утилітарних класів

1. ⬜ Визначити часто використовувані утилітарні класи Bootstrap
2. ⬜ Замінити на еквівалентні класи Tailwind CSS
3. ⬜ Створити кастомні утиліти для відсутніх еквівалентів

### Етап 5: Фінальне тестування та видалення Bootstrap

1. ⬜ Перевірити функціональність всіх сторінок
2. ⬜ Перевірити адаптивність на різних пристроях
3. ⬜ Видалити Bootstrap залежності
4. ⬜ Оптимізувати кінцевий CSS файл Tailwind

## Поточний стан

Прогрес міграції:
- Базовий фреймворк для міграції встановлено і працює
- Tailwind CSS підключено до проєкту і компілюється без помилок
- Створено шар сумісності з Bootstrap для поступової міграції
- Мігровано верхню та ліву панелі на Tailwind CSS
- Оновлено систему переключення між темною та світлою темами

Наступні кроки:
1. Продовжити міграцію компонентів правої панелі
2. Оновити модальні вікна та форми
3. Замінити сіткову систему Bootstrap на Tailwind Flex/Grid

## Карта відповідності класів

### Сіткова система

| Bootstrap | Tailwind CSS |
|-----------|--------------|
| `.container` | `.container mx-auto` |
| `.row` | `.flex flex-wrap` |
| `.col` | `.flex-1` |
| `.col-md-6` | `.md:w-1/2` |
| `.col-lg-4` | `.lg:w-1/3` |
| `.col-12` | `.w-full` |

### Компоненти

| Bootstrap | Tailwind CSS |
|-----------|--------------|
| `.btn` | `.py-2 px-4 rounded` |
| `.btn-primary` | `.bg-blue-500 text-white hover:bg-blue-600` |
| `.btn-secondary` | `.bg-gray-500 text-white hover:bg-gray-600` |
| `.alert` | `.p-4 rounded` |
| `.card` | `.rounded overflow-hidden shadow` |
| `.navbar` | `.flex items-center justify-between p-4` |

### Утиліти

| Bootstrap | Tailwind CSS |
|-----------|--------------|
| `.d-flex` | `.flex` |
| `.justify-content-between` | `.justify-between` |
| `.align-items-center` | `.items-center` |
| `.text-center` | `.text-center` |
| `.mt-3` | `.mt-3` |
| `.p-2` | `.p-2` |
| `.bg-primary` | `.bg-blue-500` |
| `.text-white` | `.text-white` |

### Медіа-запити (адаптивність)

| Bootstrap | Tailwind CSS |
|-----------|--------------|
| `@media (min-width: 576px)` | `sm:` prefix (640px) |
| `@media (min-width: 768px)` | `md:` prefix (768px) |
| `@media (min-width: 992px)` | `lg:` prefix (1024px) |
| `@media (min-width: 1200px)` | `xl:` prefix (1280px) |
| `@media (min-width: 1400px)` | `2xl:` prefix (1536px) |

## Ресурси

- [Tailwind CSS документація](https://tailwindcss.com/docs)
- [Інструмент міграції з Bootstrap на Tailwind](https://github.com/awssat/tailwindo)
- [Шпаргалка з класів Tailwind](https://nerdcave.com/tailwind-cheat-sheet) 