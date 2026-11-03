# 📸 Keepsake — Responsive Landing Page

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live%20Demo-brightgreen?style=for-the-badge&logo=github)](https://alisaartemenko.github.io/landing_keepsake/)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)

Адаптивний односторінковий лендінг для фотоагенції **Keepsake**, розроблений за макетом Figma з дотриманням найсучасніших верстальних стандартів без використання JavaScript (Pure CSS).

🔗 **Live Demo:** [https://alisaartemenko.github.io/landing_keepsake/](https://alisaartemenko.github.io/landing_keepsake/)

---

## 🎨 Особливості та UI States

- **Mobile First Approach:** Базова адаптивність орієнтована на мобільні пристрої від `375px`, із плавним розширенням під планшети (`768px`) та десктопи (`1280px`).
- **Interactive UI (No JS):**
  - **Бургер-меню:** Реалізовано через CSS-патерн `input[type="checkbox"]:checked ~ .menu`.
  - **Фільтр портфоліо:** Інтерактивне перемикання категорій робіт за допомогою `input[type="radio"]:checked ~`.
  - **Модалка Success:** Відображення успішної відправки форми через псевдоклас `:target`.
  - **Валідація форми:** Стилізація помилок вводу за допомогою сучасного псевдокласу `:user-invalid`.
- **Ховер та Фокус:** Повна доступність для клавіатурного вводу та стилізація карток портфоліо через комбінацію `:hover` + `:focus-within`.

---

## 🛠 Технології та архітектурні рішення

- **Семантичний HTML5:** Чітка структура документа з використанням тегів `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`, `<form>`. Дотримано ієрархію заголовків — суворо один `<h1>` на сторінку.
- **CSS-змінні (`:root`):** Усі кольори, шрифти, базові відступи та розміри винесені в змінні. На медіа-запитах перевизначаються **лише змінні**, що забезпечує чистоту і легку підтримку коду.
- **Розкладка:** 
  - **Flexbox** — для навігації, блоків та компонентів.
  - **CSS Grid** — виключно для сітки портфоліо із використанням власності `aspect-ratio` для ідеального збереження пропорцій карток.
- **Типографіка:** Шрифти `Oswald`, `Open Sans` та `Dancing Script` підключені з Google Fonts із параметром `display=swap` для оптимізації завантаження.
- **Графіка:** Оптимізовані інлайн SVG-іконки для максимальної швидкодії та відсутності зайвих HTTP-запитів.
- **Допоміжні елементи:** Фіксований `<header>` при скролі та CSS-кнопка вгору стандартизованого розміру `44×44px`.

---

## 📐 Брейкпоінти та Макет

| Девайс | Брейкпоінт | Основна сітка / Контейнер |
| :--- | :--- | :--- |
| **Mobile** | `375px` | 1 колонка, гумова ширина |
| **Tablet** | `768px` | Адаптивна сітка |
| **Desktop** | `1280px` | `max-width: 1100px` (центрування `margin: 0 auto`) |

---

## 🚀 Публікація та розгортання

Для деплою проєкту на **GitHub Pages** виконайте наступні команди в терміналі:

```bash
# Ініціалізація та коміт
git init
git add .
git commit -m "Keepsake landing page initial commit"

# Налаштування гілки та віддаленого репозиторію
git branch -M main
git remote add origin [https://github.com/YOUR-USERNAME/landing_keepsake.git](https://github.com/YOUR-USERNAME/landing_keepsake.git)

# Відправка коду на GitHub
git push -u origin main
