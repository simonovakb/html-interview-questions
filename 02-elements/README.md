# HTML elements

Ниже приведён набор вопросов и кратких ответов по теме «HTML Elements» - тегов и их структуры, работы с содержимым, атрибутов и распространённых практик.

---

## Вопросы:

<details>
  <summary>1. Что такое HTML‑элемент?</summary>

  HTML‑элемент состоит из тега (например, `<div>`), его атрибутов и содержимого. Элементы используются для структурирования и описания содержимого веб‑страницы.

</details>

<details>
  <summary>2. Какие бывают основные типы элементов в HTML?</summary>

  Есть блочные (`<div>`, `<section>`, `<article>`) и строчные (`<span>`, `<a>`, `<strong>`); а также эмблемные (например, `<img>`, `<input>`).

</details>

<details>
  <summary>3. Как вложенность работает в HTML‑элементах?</summary>

  Элементы HTML могут содержать другие элементы и текст. Вложенность формирует DOM-дерево, где каждый уровень — вложенный тег.

</details>

<details>
  <summary>4. Какие атрибуты встречаются у HTML‑элементов?</summary>

  Атрибуты (например, `id`, `class`, `title`, `data-*`, `style`) определяют дополнительные свойства, идентификаторы и оформление элемента.

</details>

<details>
  <summary>5. Чем отличается self‑closing элемент от парного?</summary>

  Self‑closing элементы (например, `<img>`, `<br>`, `<hr>`) не содержат закрывающего тега. Парные элементы требуют закрывающего (например, `<div></div>`).

</details>

<details>
  <summary>6. Для чего используется атрибут class?</summary>

  Атрибут `class` позволяет присваивать элементу один или несколько CSS‑классов для стилизации и JS‑работы с группой элементов.

</details>

<details>
  <summary>7. Как работает атрибут id? В чём разница с class?</summary>

  `id` уникален для всей страницы и используется для идентификации элемента (например, для якорей, скриптов). `class` можно применять к нескольким элементам.

</details>

<details>
  <summary>8. Что делают тег &lt;span&gt; и тег &lt;div&gt;?</summary>

  `<span>` — строчный контейнер, используется для выделения части текста или инлайнового фрагмента. `<div>` — блочный контейнер для группировки элементов/контента.

</details>

<details>
  <summary>9. Для чего служит тег &lt;a&gt;? Какие атрибуты у него важны?</summary>

  `<a>` задаёт ссылку. Важные атрибуты: `href` (адрес), `target` (как открывать), `rel` (безопасность), `download` (скачивание).

</details>

<details>
  <summary>10. Как работает тег &lt;img&gt; и какие у него есть обязательные атрибуты?</summary>

  `<img>` вставляет изображение. Обязательны: `src` (путь к картинке), `alt` (описание для доступности и SEO); опционально: `width`, `height`, `loading`.

</details>

<details>
  <summary>11. Как работать с элементами списка (&lt;ul&gt;, &lt;ol&gt;, &lt;li&gt;)?</summary>

  `<ul>` — маркированный, `<ol>` — нумерованный список; внутри идут `<li>` — элементы списка. Списки помогают структурировать информацию.

</details>

<details>
  <summary>12. Для чего используется тег &lt;form&gt; и вложенные элементы?</summary>

  `<form>` объединяет поля для ввода данных, кнопки; позволяет отправлять информацию на сервер. Внутри часто: `<input>`, `<select>`, `<textarea>`, `<button>`.

</details>

<details>
  <summary>13. Какие есть специальные HTML‑элементы для работы с таблицами?</summary>

  `<table>` — таблица, вложенные: `<tr>` (строка), `<td>` (ячейка данных), `<th>` (заголовок), `<thead>`, `<tbody>`, `<tfoot>` для структуры.

</details>

<details>
  <summary>14. Что такое вложенные элементы форм (Fieldset, Legend)?</summary>

  `<fieldset>` группирует связанные поля формы, `<legend>` задаёт подпись группы, повышая доступность.

</details>

<details>
  <summary>15. Как добавить интерактивность с помощью button‑элемента?</summary>

  `<button>` создаёт кнопку. Атрибуты: `type` (`submit`, `button`, `reset`), `disabled` (деактивация). Для событий используется JS.

</details>

<details>
  <summary>16. Какие элементы применяют для вставки мультимедиа?</summary>

  `<img>` для изображений, `<audio>` для аудио, `<video>` для видео; поддерживают дополнительные атрибуты (контроль, источники).

</details>

<details>
  <summary>17. Что делает тег &lt;iframe&gt; и как ограничить его возможности?</summary>

  `<iframe>` встраивает внешнее содержимое (другой сайт, документ); атрибуты безопасности: `sandbox`, `allow`.

</details>

<details>
  <summary>18. В чём особенности применения тегов &lt;strong&gt;, &lt;em&gt;, &lt;mark&gt;?</summary>

  `<strong>` — важность, выделяет жирным, `<em>` — акцент (курсив), `<mark>` — подчеркивает текст (выделение фоном).

</details>

<details>
  <summary>19. Какие особенности у элемента &lt;input&gt;?</summary>

  `<input>` — поле для ввода; поддерживает типы (`text`, `password`, `email`, `checkbox`, `radio`, `range` и др.), атрибуты валидации (`required`, `pattern`, `min`, `max`).

</details>

<details>
  <summary>20. Что такое пустые элементы? Примеры</summary>

  Элементы без содержимого: `<br>`, `<hr>`, `<img>`, `<input>`. Они либо оформляют разметку, либо несут медиа/инпут.

</details>

<details>
  <summary>21. Как работает тег &lt;label&gt; и почему он важен для форм?</summary>

  `<label>` связывает описание с элементом ввода (`input`/`select`), обеспечивает доступность (по клику фокусирует на поле).

</details>

<details>
  <summary>22. Для чего используют тег &lt;select&gt;?</summary>

  `<select>` создаёт раскрывающийся список опций; `<option>` — варианты выбора, может быть группировка через `<optgroup>`.

</details>

<details>
  <summary>23. Как задать заголовки через h1‑h6 и почему важна их иерархия?</summary>

  Заголовки `<h1>`‑`<h6>` передают структуру документа для SEO и доступности; корректная иерархия облегчает навигацию и восприятие.

</details>

<details>
  <summary>24. Какие HTML‑элементы используются для текстовой разметки?</summary>

  `<p>` — абзац, `<br>` — перенос, `<blockquote>` — цитата, `<strong>` — важное, `<em>` — акцент, `<sup>`/`<sub>` — индексы.

</details>

<details>
  <summary>25. Как работают data‑атрибуты у HTML‑элементов?</summary>

  `data-*` позволяют хранить любые пользовательские данные, обращаться к ним из JS (например, `element.dataset.myValue`).

</details>

<details>
  <summary>26. Что такое deprecated и obsolete‑элементы?</summary>

  Deprecated — устаревшие теги/атрибуты (например, `<font>`, `<center>`); их поддержка постепенно прекращается, заменяются CSS и современными тегами.

</details>

<details>
  <summary>27. Что такое contenteditable?</summary>

  Атрибут `contenteditable` делает элемент редактируемым пользователем прямо на странице (например, для простых админок/редакторов).

</details>

<details>
  <summary>28. Для чего используются aria‑атрибуты у элементов?</summary>

  `aria-*` атрибуты помогают адаптировать элементы для вспомогательных технологий (читают описание, роль, состояние; улучшается a11y).

</details>

<details>
  <summary>29. Как выбрать элемент в JS через селекторы?</summary>

  Используйте `document.getElementById`, `getElementsByClassName`, `getElementsByTagName`, или современные `querySelector`/`querySelectorAll`.

</details>

<details>
  <summary>30. Что такое кастомные элементы (Web Components) — &lt;my-element&gt;?</summary>

  В HTML5 можно создавать собственные теги (Web Components, custom elements) через JS: `customElements.define('my-element', ...)`. Они позволяют инкапсулировать поведение/стили.
</details>

<details>
  <summary>31. Для чего используются теги &lt;main&gt;, &lt;aside&gt;, &lt;nav&gt;?</summary>
  Они дают структуру и смысл странице, помогают screen reader-ам определить основные части интерфейса (основной контент, навигация, боковые панели).
</details>

<details>
  <summary>32. Как работают элементы &lt;script&gt; и &lt;link&gt;?</summary>

  - `<script>` подключает JS, атрибуты `src`, `type`, `defer`, `async`
  - `<link>` — для стилей, шрифтов, prefetch/preload.

</details>

<details>
  <summary>33. Можно ли вставлять SVG или MathML непосредственно в HTML?</summary>

  Да, `<svg>` и `<math>` — встроенные стандарты, помогают для графики и формул прямо в DOM.

</details>

<details>
  <summary>34. Для чего служат теги &lt;time&gt; и &lt;meter&gt;, &lt;progress&gt;?</summary>

  `<time>` — машиночитаемая разметка дат/времени. `<meter>`, `<progress>` — отображение значения метрики или прогресса.

</details>

<details>
  <summary>35. Как можно навесить обработчик события непосредственно через HTML‑атрибут?</summary>

  Можно использовать атрибут `onclick`, `onchange` и др., но лучше навешивать через JS.

</details>

<details>
  <summary>36. Как добавить микроразметку schema.org — через какие атрибуты?</summary>

  Используют `itemscope`, `itemtype`, `itemprop` для структурирования данных (например: `<div itemscope itemtype="https://schema.org/Product">`).

</details>

<details>
  <summary>37. Что такое role‑атрибут и когда его использовать?</summary>
  
  Атрибут `role` описывает назначение элемента для вспомогательных технологий. Например: `role="button"`, `role="navigation"`.

</details>

<details>
  <summary>38. Для чего нужны &lt;figure&gt; и &lt;figcaption&gt;?</summary>

  `<figure>` группирует медиа‑контент, `<figcaption>` — подпись. Улучшает семантику и доступность.

</details>

<details>
  <summary>39. Какие ещё важные атрибуты для доступности — кроме aria?</summary>

  `tabindex`, `title`, `alt`, а также правильная структура навигации и заголовков.

</details>

<details>
  <summary>40. В чём разница между &lt;b&gt; и &lt;strong&gt;?</summary>

  - <b>&lt;b&gt;</b> - просто визуально выделяет текст жирным, без дополнительного смысла (presentational).
  - <strong>&lt;strong&gt;</strong> - подчеркивает важность (semantic), сообщает скринридерам о акценте, может влиять на SEO и доступность.

</details>

<details>
  <summary>41. В чём разница между &lt;i&gt; и &lt;em&gt;?</summary>

  - <i>&lt;i&gt;</i> — меняет стиль на курсив, не несёт семантики (presentational).  
  - <em>&lt;em&gt;</em> — выделяет акцент, смысловой упор, делает текст более заметным для вспомогательных технологий.

</details>

<details>
  <summary>42. В чём практическая разница между &lt;strong&gt;, &lt;em&gt;, &lt;mark&gt;?</summary>

  - <strong>&lt;strong&gt;</strong> — важность, акцент для a11y (скринридеров), SEO.  
  - <em>&lt;em&gt;</em> — смысловой акцент, интонация.  
  - <mark>&lt;mark&gt;</mark> — визуальное выделение фона, обычно для поиска или подсветки.

</details>

<details>
  <summary>43. Отличие между &lt;button&gt; и &lt;input type="button"&gt;?</summary>

  - <button>&lt;button&gt;</button> может содержать HTML (иконки, текст), поддерживает любые вложенные элементы, атрибуты `type` ("button", "submit", "reset"), стилизуется простым CSS и более гибок для a11y.
  - <input type="button" /> отображает только текст (через value), нельзя вставить HTML внутри, есть только `type="button"` (нет submit/reset). Менее гибок для стилизации и доступности.

</details>


<details>
  <summary>44. Когда использовать &lt;button&gt;, а когда &lt;input type="button"&gt;?</summary>

  - Для современных веб-приложений — рекомендуется `<button/>` (гибкость, доступность, вложения, поддержка submit/reset).  
  - `<input type="button"/>` — для простых сценариев, совместимости с очень старым кодом.

</details>

<details>
  <summary>45. Как влияет выбор между presentational и semantic elements на доступность?</summary>

  - Семантические теги (`<strong>`, `<em>`, `<button>`) увеличивают доступность и корректную работу вспомогательных технологий.
  - Presentational (`<b>`, `<i>`, `<input type="button">`) только визуально изменяют текст, не добавляя смысл.

</details>