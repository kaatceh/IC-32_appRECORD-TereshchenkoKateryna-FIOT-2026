## Тема, Мета, Місце розташування

**Тема:** Назва лабораторної роботи.

**Мета:** Коротко описати мету.

**Місце розташування:**
- GitHub: (встав посилання)
- Live demo: (встав посилання)
- Репозиторій звітного HTML-документа (GitHub): 
https://github.com/kaatceh/IC-32_appRECORD-TereshchenkoKateryna-FIOT-2026
- Звітний HTML-документ (Жива сторінка)
https://kaatceh.github.io/IC-32_appRECORD-TereshchenkoKateryna-FIOT-2026/

---

## Опис предметного середовища

**Предметна галузь:** система керування студентськими нотатками. Веб-застосунок дозволяє користувачу переглядати нотатки, організовані у вигляді інформаційних карток, а також використовувати навігацію для переходу між розділами сайту.

---

## Структура веб-застосунку

- **Головна сторінка** — містить вступну інформацію та загальний вигляд застосунку.
- **Нотатки** — відображення списку нотаток у вигляді карток.
- **Можливості** — опис функціоналу системи.
- **Контакти** — довідкова інформація.

---

## Сценарій взаємодії (бізнес-логіка)

1. Користувач відкриває веб-застосунок.
2. Переглядає головну сторінку.
3. Переходить до розділу «Нотатки».
4. Ознайомлюється з картками нотаток.
5. Використовує навігаційне меню для переходу між розділами.
6. На мобільних пристроях використовує бургер-меню.
7. Взаємодіє з елементами інтерфейсу.

---

## Функціональні вимоги

- Відображення головної сторінки.
- Наявність header, main та footer.
- Відображення нотаток у вигляді карток.
- Навігаційне меню між розділами.
- Реалізація бургер-меню.
- Адаптивне відображення контенту.
- Наявність інтерактивних елементів (кнопки, hover-ефекти).

---

## Нефункціональні вимоги

- Адаптивність інтерфейсу.
- Зручність використання.
- Швидке завантаження сторінки.
- Кросбраузерність.
- Простий та зрозумілий дизайн.

---

## Стек технологій

- HTML5 — структура сторінки.
- CSS3 — стилізація та адаптивність (flexbox, grid, media queries).
- JavaScript — інтерактивність.
- Git / GitHub — контроль версій.
- GitHub Pages — публікація.

---

## Структура документа

Нижче наведено узагальнену структуру HTML сторінки веб-застосунку.

```<!DOCTYPE html>
<html lang="uk">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Student Notes System</title>
  <link rel="stylesheet" href="./css/style.css" />
</head>
<body>
  <header class="header">
    <div class="container header__container">
      <div class="logo">Student Notes</div>

      <button class="burger" id="burger" aria-label="Відкрити меню">
        <span></span>
        <span></span>
        <span></span>
      </button>

      <nav class="nav" id="nav">
        <a href="#home" class="nav__link">Головна</a>
        <a href="#notes" class="nav__link">Нотатки</a>
        <a href="#features" class="nav__link">Можливості</a>
        <a href="#contacts" class="nav__link">Контакти</a>
      </nav>
    </div>
  </header>

  <main>
    <section class="hero" id="home">
      <div class="container">
        <h1 class="hero__title">Student Notes System</h1>
        <p class="hero__text">
          Адаптивний web-застосунок для зручного керування студентськими нотатками.
        </p>
        <a href="#notes" class="button">Переглянути нотатки</a>
      </div>
    </section>

    <section class="notes" id="notes">
      <div class="container">
        <h2 class="section-title">Мої нотатки</h2>

        <div class="cards">
          <article class="card">
            <h3 class="card__title">Лекція з веб-розробки</h3>
            <p class="card__text">
              Основи HTML, CSS та JavaScript. Семантичні теги, адаптивна верстка.
            </p>
            <button class="card__button">Детальніше</button>
          </article>

          <article class="card">
            <h3 class="card__title">План на тиждень</h3>
            <p class="card__text">
              Завершити лабораторну роботу, оформити GitHub-репозиторій та README.
            </p>
            <button class="card__button">Детальніше</button>
          </article>

          <article class="card">
            <h3 class="card__title">Ідеї для проєкту</h3>
            <p class="card__text">
              Додати категорії нотаток, пошук, фільтри та авторизацію користувача.
            </p>
            <button class="card__button">Детальніше</button>
          </article>

          <article class="card">
            <h3 class="card__title">Нагадування</h3>
            <p class="card__text">
              Перевірити адаптивність сторінки для смартфона, планшета і десктопа.
            </p>
            <button class="card__button">Детальніше</button>
          </article>

          <article class="card">
            <h3 class="card__title">UI-елементи</h3>
            <p class="card__text">
              Реалізувати бургер-меню, hover-ефекти та плавну анімацію появи карток.
            </p>
            <button class="card__button">Детальніше</button>
          </article>

          <article class="card">
            <h3 class="card__title">Git-коміти</h3>
            <p class="card__text">
              Створити логічні коміти: header, cards layout, burger menu, responsive styles.
            </p>
            <button class="card__button">Детальніше</button>
          </article>
        </div>
      </div>
    </section>

    <section class="features" id="features">
      <div class="container">
        <h2 class="section-title">Можливості системи</h2>
        <div class="features__list">
          <div class="feature-item">Адаптивний інтерфейс</div>
          <div class="feature-item">Зручна навігація</div>
          <div class="feature-item">Сітка карток</div>
          <div class="feature-item">Анімації та hover-ефекти</div>
        </div>
      </div>
    </section>
  </main>

  <footer class="footer" id="contacts">
    <div class="container">
      <p>© 2026 Student Notes System</p>
      <p>Email: studentnotes@example.com</p>
    </div>
  </footer>

  <script src="./js/script.js"></script>
</body>
</html>

## Хід виконання

## Фрагменти коду

### HTML (навігація та структура)

```html
<header class="header">
  <div class="logo">Student Notes</div>

  <nav class="nav">
    <ul class="menu">
      <li><a href="#">Головна</a></li>
      <li><a href="#">Нотатки</a></li>
      <li><a href="#">Можливості</a></li>
      <li><a href="#">Контакти</a></li>
    </ul>
  </nav>

  <div class="burger">
    ☰
  </div>
</header>

<main>
  <div class="cards">
    <div class="card">
      <h3>Нотатка 1</h3>
      <p>Опис нотатки</p>
    </div>
  </div>
</main>

<footer>
  Контакти
</footer>

## Скріншоти

![Головна](/assets/labs/lab-1/screen-1.png)
![Мобільна](/assets/labs/lab-1/screen-2.png)

---
## Use-case діаграма

![Use-case](/assets/labs/lab-1/usecase.png)

Use-case діаграма відображає основні сценарії взаємодії користувача з веб-застосунком. 
Користувач може переглядати сторінки сайту, переглядати нотатки, здійснювати навігацію між розділами та використовувати меню.

---

## ER-діаграма

![ER](/assets/labs/lab-1/er.png)

ER-діаграма відображає основні сутності системи та зв’язки між ними. 
Сутність «Користувач» пов’язана із сутністю «Нотатка» зв’язком один-до-багатьох (1:N).

---

## Висновки

У ході виконання лабораторної роботи було розроблено адаптивний веб-застосунок для керування студентськими нотатками.

Було реалізовано структуру веб-сторінки з використанням HTML, стилізацію та адаптивну верстку за допомогою CSS (flexbox, grid, media queries), а також інтерактивність за допомогою JavaScript (бургер-меню).

Побудовано Use-case діаграму, що відображає основні сценарії взаємодії користувача із системою, та ER-діаграму, яка описує структуру даних і зв’язки між сутностями.

Отримано практичні навички створення адаптивних інтерфейсів, роботи з GitHub та оформлення звітів у Markdown з подальшою публікацією через GitHub Pages.
