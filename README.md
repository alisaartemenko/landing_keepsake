# Keepsake – responsive landing

**Demo:** https://YOUR-USERNAME.github.io/landing-keepsake/

Адаптивний односторінковий лендінг агенції Keepsake за макетом Figma (Desktop 1280 / Tablet 768 / Mobile 375 / menu open / UI states).

## Технології та рішення
- Семантичний HTML5 (`header`, `nav`, `main`, `section`, `article`, `footer`, `form`), один `h1`.
- CSS-змінні в `:root` (кольори, шрифти, відступи, розміри) — на брейкпоінтах змінюються лише змінні.
- Mobile first: `@media (min-width: 768px)` та `(min-width: 1280px)`; контейнер max 1100px.
- Flexbox для розкладки; CSS Grid лише для сітки робіт (`aspect-ratio` для карток).
- Без JS: бургер-меню — `input:checked ~ .menu`; фільтр портфоліо — `radio:checked ~`; success форми — `:target`; error — `:user-invalid`.
- Ховер/focus карточки: `:hover` + `:focus-within`.
- Інлайн-SVG іконки, шрифти Oswald / Open Sans / Dancing Script з Google Fonts (`display=swap`).
- Фіксований header, кнопка «вгору» 44×44.

## Публікація на GitHub Pages
```bash
git init && git add . && git commit -m "Keepsake landing"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/landing-keepsake.git
git push -u origin main
```
Settings → Pages → Source: *Deploy from a branch* → `main` / `/ (root)`.
