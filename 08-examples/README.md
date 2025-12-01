# Готовые примеры и шаблоны HTML

Набор готовых сниппетов, шаблонов и структур для типовой HTML-верстки. Быстрое повторение базовых приёмов и современных паттернов.

---

## Вопросы и практические примеры:

<details>
  <summary>1. Базовая структура HTML5 документа</summary>

  ```html
  <!DOCTYPE html>
  <html lang="ru">
    <head>
      <meta charset="utf-8">
      <meta name="viewport" content="width=device-width, initial-scale=1">
      <title>Заголовок страницы</title>
    </head>
    <body>
      <!-- Контент здесь -->
    </body>
  </html>
  ```
</details>

<details>
  <summary>2. Семантическая разметка основной страницы</summary>

  ```html
  <header>
    <nav>
      <ul>
        <li><a href="#">Главная</a></li>
        <li><a href="#">О нас</a></li>
      </ul>
    </nav>
  </header>
  <main>
    <article>
      <h1>Заголовок статьи</h1>
      <p>Основной текст...</p>
    </article>
    <aside>
      Боковая информация
    </aside>
  </main>
  <footer>
    &copy; 2025 Пример сайта
  </footer>
  ```
</details>

<details>
  <summary>3. Пример изображения с адаптивной загрузкой</summary>

  ```html
  <picture>
    <source srcset="image.avif" type="image/avif">
    <source srcset="image.webp" type="image/webp">
    <img src="image.jpg" alt="Описание изображения" width="640" height="320" loading="lazy">
  </picture>
  ```
</details>

<details>
  <summary>4. Готовая форма с доступностью и валидацией</summary>

  ```html
  <form action="#" method="post" autocomplete="on">
    <fieldset>
      <legend>Регистрация</legend>
      <label for="email">Email:</label>
      <input id="email" name="email" type="email" required autocomplete="email">

      <label for="pass">Пароль:</label>
      <input id="pass" name="password" type="password" required minlength="6">

      <button type="submit">Отправить</button>
    </fieldset>
  </form>
  ```
</details>

<details>
  <summary>5. Карточка с изображением и подписью (figure/figcaption)</summary>

  ```html
  <figure>
    <img src="cat.jpg" alt="Кот у окна" width="300" height="200">
    <figcaption>Луч солнца золотого...</figcaption>
  </figure>
  ```
</details>

<details>
  <summary>6. Пример видео с постером и субтитрами</summary>

  ```html
  <video width="320" height="240" controls poster="preview.jpg">
    <source src="movie.mp4" type="video/mp4">
    <source src="movie.webm" type="video/webm">
    <track kind="subtitles" src="subs_ru.vtt" srclang="ru" label="Русский">
    Ваш браузер не поддерживает видео.
  </video>
  ```
</details>

<details>
  <summary>7. Чек-лист мета-тегов для head</summary>

  ```html
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="description" content="Описание страницы до 160 символов">
    <meta name="theme-color" content="#336699">
    <meta name="robots" content="index,follow">
    <meta property="og:title" content="Название страницы">
    <meta property="og:description" content="OG-описание">
    <link rel="icon" href="/favicon.ico">
    <link rel="canonical" href="https://site.ru/page">
    <link rel="manifest" href="/manifest.json">
  </head>
  ```
</details>

<details>
  <summary>8. Модальное окно с управлением фокусом и aria-атрибутами</summary>

  ```html
  <div class="modal" role="dialog" aria-modal="true" aria-labelledby="modalTitle" tabindex="-1">
    <h2 id="modalTitle">Заголовок окна</h2>
    <p>Текст внутри модального окна.</p>
    <button type="button" aria-label="Закрыть">Закрыть</button>
  </div>
  ```
</details>

<details>
  <summary>9. Пример списка с группировкой (select/optgroup)</summary>

  ```html
  <select>
    <optgroup label="Фрукты">
      <option>Яблоко</option>
      <option>Груша</option>
    </optgroup>
    <optgroup label="Овощи">
      <option>Томат</option>
      <option>Огурец</option>
    </optgroup>
  </select>
  ```
</details>

<details>
  <summary>10. Карта/интерактивная область (map/area)</summary>

  ```html
  <img src="plan.jpg" usemap="#office-map" alt="План офиса">
  <map name="office-map">
    <area shape="rect" coords="34,44,270,350" href="room1.html" alt="Первая комната">
    <area shape="circle" coords="337,300,44" href="kitchen.html" alt="Кухня">
  </map>
  ```
</details>