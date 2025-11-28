# HTML База

Набор вопросов и кратких ответов по HTML для подготовки к собеседованию.

Этот документ - справочник и шпаргалка по HTML для подготовки к собеседованию и быстрого повторения. В нём собраны:
- Раздел "HTML База" с вопросами и сжатыми ответами (семантика, структура документа, meta‑теги, формы, безопасность, производительность и т.д.).  
- Расширенные/углублённые темы для среднего и senior‑уровней (PWA, Service Worker, SRI, Critical Rendering Path и пр.). 

---

## Вопросы:

<details>
  <summary>1. Что такое <em>HTML</em> и для чего он используется?</summary>

  `HTML` — это язык разметки для описания структуры веб‑страниц и их семантики; в связке с `CSS` и `JavaScript` он формирует интерфейс и поведение веб‑приложений.

</details>

<details>
  <summary>2. Чем <em>HTML</em> отличается от <em>HTML5</em>?</summary>

  `HTML5` — современная спецификация языка `HTML`, которая включает семантические теги, расширенную поддержку мультимедиа и новые `API` (`Canvas`, `WebSocket`, геолокация и др.).

</details>

<details>
  <summary>3. Что такое семантические теги и зачем они нужны?</summary>

  Теги вроде `<header>`, `<nav>`, `<article>` дают смысл структуре страницы, улучшают доступность и `SEO`.

</details>

<details>
  <summary>4. Как <em>HTML</em> влияет на доступность (<em>a11y</em>)?</summary>

  Правильная семантика и атрибуты (`aria`, `alt`) позволяют вспомогательным технологиям корректно интерпретировать страницу.

</details>

<details>
  <summary>5. Что такое <em>DOM</em>?</summary>

  `DOM` — объектная модель документа, которую браузер строит из `HTML`; `JavaScript` манипулирует DOM для динамических изменений страницы.

</details>

<details>
  <summary>6. Как <em>HTML</em> взаимодействует с <em>CSS</em> и <em>JavaScript</em>?</summary>

  - `HTML` отвечает за структуру  
  - `CSS` — за представление (стили)  
  - `JS` — за поведение (логика и динамика)  

  Они вместе формируют `UI`.

</details>

<details>
  <summary>7. Что такое <em>Doctype</em> и зачем он нужен?</summary>

  `<!DOCTYPE html>` указывает браузеру использовать современный режим парсинга/рендеринга (`HTML5`).

</details>

<details>
  <summary>8. Какие важные meta‑теги вы знаете?</summary>

  - charset — кодировка документа. Пример: `<meta charset="utf-8">`  
  - viewport — адаптивность на мобильных устройствах. Пример: `<meta name="viewport" content="width=device-width, initial-scale=1">`  
  - description — описание страницы для поисковиков. Пример: `<meta name="description" content="Краткое описание страницы до ~150–160 символов.">`  
  - robots — управление индексированием (index/noindex и т.д.). Пример: `<meta name="robots" content="index,follow">`  
  - theme-color — цвет интерфейса в мобильных браузерах. Пример: `<meta name="theme-color" content="#0d47a1">`  
  - Open Graph / Twitter Cards — мета для корректного отображения при шаринге. Пример: `<meta property="og:title" content="Заголовок">`

</details>

<details>
  <summary>9. Чем блочные и строчные элементы отличаются?</summary>

  - Блочные элементы (например, `div`, `p`) начинают новую строку, по умолчанию занимают всю доступную ширину контейнера; у них можно задавать width/height.  
  - Строчные (inline) элементы (например, `span`, `a`) располагаются в тексте, их ширина определяется содержимым; width/height обычно игнорируются.  
  - Примечание: `<p>` — блочный элемент. Для поведения между inline и block есть `display: inline-block`.

</details>

<details>
  <summary>10. Как работают формы и валидация в <em>HTML</em>?</summary>

  Формы определяются тегами `form` и `input` (и другими полями). Есть встроенная валидация (`required`, `type`, `pattern` и др.) и возможность дополнять её на клиенте/сервере через JS/серверную логику.

</details>

<details>
  <summary>11. Какие <em>HTML</em>‑фичи влияют на производительность страницы?</summary>

  Расположение скриптов (defer/async), оптимизация медиа (форматы/размеры), отложенная загрузка (lazy), минимизация и оптимизация DOM, использование preload/preconnect и критического CSS.

</details>

<details>
  <summary>12. Какие у <em>HTML</em> есть возможности для мультимедиа?</summary>

  Теги `<audio>`, `<video>`, элемент `<canvas>` для графики; поддержка медиа‑API (MediaDevices, WebRTC) и управление форматами/потоками.

</details>

<details>
  <summary>13. Что такое <em>SEO</em> и как <em>HTML</em> влияет на него?</summary>

  `SEO` — оптимизация для поисковиков; семантика, корректные заголовки, метаописания, структурированные данные (schema.org) и канонические ссылки помогают ранжированию.

</details>

<details>
  <summary>14. Есть ли риски безопасности, связанные с <em>HTML</em>?</summary>

  Да — XSS через вставку некорректного HTML/JS; защита — корректное экранирование, Content Security Policy (CSP), валидация и санитизация на сервере.

</details>

<details>
  <summary>15. Как проверить корректность <em>HTML</em>?</summary>

  Использовать валидаторы (W3C), линтеры (HTMLHint), автоматические тесты, а также инструменты для a11y (axe, Lighthouse) и ручное тестирование в браузерах.

</details>

<details>
  <summary>16. Назовите новые <em>API</em>, добавленные в <em>HTML5</em></summary>

  `Canvas`, `WebSockets`, `Web Storage (localStorage/sessionStorage)`, `Geolocation`, `MediaDevices`/`WebRTC` и другие веб‑API.

</details>

<details>
  <summary>17. Что входит в базовую структуру HTML‑документа?</summary>

  ```html
  <!DOCTYPE html>
  <html lang="ru">
    <head>
      <meta charset="utf-8">
      <title>Заголовок</title>
      <!-- meta, link, script и т.д. -->
    </head>
    <body>
      <!-- содержимое страницы -->
    </body>
  </html>
  ```
  - `<!DOCTYPE html>` включает современный режим парсинга (HTML5).  
  - В `<head>` ставятся meta‑теги, ссылки на стили, preloads и управление загрузкой скриптов.  
  - В `<body>` — видимый контент и интерактивные элементы.

</details>

<details>
  <summary>18. Чем отличается &lt;head&gt; от &lt;body&gt;?</summary>

  `<head>` содержит метаданные страницы (`meta`, `title`, `link`, `base`, рекомендации по загрузке ресурсов), а `<body>` содержит видимый контент для пользователя. Head используется браузером для настройки рендеринга.

</details>

<details>
  <summary>19. Как правильно указывать кодировку страницы? (&lt;meta charset="utf-8"&gt;)</summary>

  Ставьте `<meta charset="utf-8">` как можно раньше в `<head>` (в идеале в пределах первых ~1024 байт документа), чтобы браузер корректно распознал кодировку и не было проблем с отображением символов.

</details>

<details>
  <summary>20. Что такое атрибут alt у &lt;img&gt; и зачем он нужен?</summary>

  `alt` — текстовое описание изображения. Нужен для доступности (скрин‑ридеры), SEO и для случаев, когда изображение не загрузилось. Для чисто декоративных изображений используйте `alt=""`.

</details>

<details>
  <summary>21. Что такое responsive images и как работать с srcset / sizes / &lt;picture&gt;?</summary>

  `srcset` и `sizes` позволяют подать разные изображения в зависимости от плотности пикселей (DPR) и ширины вьюпорта; `<picture>` даёт контроль над выбором формата/источника (например, WebP/AVIF для поддерживающих браузеров).

</details>

<details>
  <summary>22. Как подключать скрипты и стили — разница между inline, external и атрибутами defer/async?</summary>

  - Inline — быстрый доступ, но снижает кэшируемость и увеличивает HTML.  
  - External — лучше кэшируются и легче поддерживаются.  
  - `defer` — загружает скрипт параллельно и выполняет после парсинга HTML (не блокирует рендер).  
  - `async` — загружает параллельно и выполняет сразу после загрузки (может прерывать парсинг).  

  Для стилей внешние `<link rel="stylesheet">` блокируют рендер, поэтому применяют критический CSS, `preload` и прочие техники.

</details>

<details>
  <summary>23. Что такое rel="noopener noreferrer" и зачем его использовать для &lt;a target="_blank"&gt;?</summary>

  `rel="noopener noreferrer"` предотвращает доступ открытой страницы к `window.opener` (защищая от tabnabbing) и (при использовании `noreferrer`) отключает передачу реферера. Рекомендуется для всех ссылок с `target="_blank"`.

</details>

<details>
  <summary>24. Что делает атрибут loading="lazy" у &lt;img&gt; и &lt;iframe&gt;?</summary>

  `loading="lazy"` откладывает загрузку ресурса до приближения его к области видимости пользователя, что экономит трафик и улучшает скорость начального рендера.

</details>

<details>
  <summary>25. Что такое canonical link (&lt;link rel="canonical"&gt;) и зачем он нужен?</summary>

  `<link rel="canonical" href="...">` указывает канонический URL страницы и помогает поисковым системам выбирать версию для индексации, уменьшая проблемы с дублированием контента.

</details>

<details>
  <summary>26. Как правильно указывать язык документа (&lt;html lang="ru"&gt;) и direction (dir)?</summary>

  Указывайте `lang` в `<html>` для доступности, корректного произношения синтезатора речи и SEO. `dir="ltr"` или `dir="rtl"` задают направление текста; `rtl` используется для языков с письмом справа налево.

</details>

<details>
  <summary>27. Что такое data-* атрибуты и где их применяют?</summary>

  `data-*` атрибуты позволяют хранить произвольные данные на элементах для использования в JavaScript без нарушения семантики (например `data-id="123"`).

</details>

<details>
  <summary>28. Что такое &lt;template&gt; и чем он полезен?</summary>

  `<template>` хранит фрагмент DOM, который не рендерится до тех пор, пока его не клонируют через JS — удобно для шаблонов UI.

</details>

<details>
  <summary>29. Что делает атрибут tabindex и как его использовать правильно?</summary>

  `tabindex` управляет порядком фокусировки: `tabindex="0"` — включить в естественный порядок; `tabindex="-1"` — убрать из таба, но доступен программно; положительные значения управляют конкретным порядком (использовать с осторожностью).

</details>

<details>
  <summary>30. Какие атрибуты важны для форм (name, action, method, autocomplete, novalidate)?</summary>

  - `name` — имя поля при отправке.  
  - `action` — куда отправлять данные.  
  - `method` — GET/POST.  
  - `autocomplete` — подсказки браузера.  
  - `novalidate` — отключает встроенную валидацию.  
  - Встроенные проверки: `required`, `pattern`, `min`, `max`, `type` и др.

</details>

<details>
  <summary>31. Что такое semantic vs presentational HTML?</summary>

  Семантические теги несут смысл (например `<article>`, `<nav>`, `<strong>`); presentational теги управляют только видом (устаревшие `<font>`, атрибуты оформления) — их заменяют CSS.

</details>

<details>
  <summary>32. Как работают атрибуты для медиа (&lt;video controls preload poster&gt;)?</summary>

  - `controls` — показывает элементы управления.  
  - `preload` — hint для предзагрузки (`auto`, `metadata`, `none`).  
  - `poster` — изображение до начала воспроизведения.  
  Настройки влияют на трафик и UX.

</details>

<details>
  <summary>33. Что такое iframe sandbox и атрибуты allow?</summary>

  `sandbox` ограничивает привилегии встроенного содержимого; `allow` и `allowfullscreen` дают конкретные разрешения (например, `allow="camera; microphone"`).

</details>

<details>
  <summary>34. Что такое microdata / schema.org и зачем это добавлять в HTML?</summary>

  Microdata / schema.org помогают разметить содержимое для поисковых систем (рецензии, события, рецепты) и повышают шанс получения богатых сниппетов.

</details>

<details>
  <summary>35. Что такое contenteditable и когда его не стоит использовать?</summary>

  `contenteditable` делает элемент редактируемым пользователем; подходит для простых задач, но для сложных редакторов лучше использовать специализированные решения (из‑за безопасности, формата и валидации).

</details>

<details>
  <summary>36. Как работать с формами и безопасностью — XSS и escaping в контексте HTML?</summary>

  Никогда не вставляйте неподготовленные данные в HTML; экранируйте ввод, используйте `textContent`/безопасные шаблонизаторы, применяйте CSP и серверную санитизацию.

</details>

<details>
  <summary>37. Что делает &lt;link rel="preload"&gt;, &lt;prefetch&gt;, &lt;preconnect&gt; и когда их применять?</summary>

  - `preload` — загружает критический ресурс для текущей страницы.  
  - `prefetch` — загружает ресурс для будущих навигаций (низкий приоритет).  
  - `preconnect` — заранее устанавливает соединение/DNS/TLS с доменом.  
  Используйте для оптимизации критического пути.

</details>

<details>
  <summary>38. Как тестировать и валидировать HTML (W3C, линтеры, accessibility tools)?</summary>

  Инструменты: W3C Validator, HTMLHint, eslint-plugin-html, axe, Lighthouse, NVDA/VoiceOver и другие a11y‑инструменты.

</details>

<details>
  <summary>39. Что такое Web App Manifest и зачем он нужен (PWA)?</summary>

  `manifest.json` описывает метаданные PWA (иконки, имя, цвет темы, режим запуска) и позволяет устанавливать сайт как приложение.

</details>

<details>
  <summary>40. Что такое Service Worker и как он связан с HTML/ресурсами?</summary>

  Service Worker — фоновой скрипт, который перехватывает сетевые запросы, обеспечивает офлайн‑режим и расширенные возможности кеширования; регистрируется через JS.

</details>

<details>
  <summary>41. Различие между мета‑тегами и HTTP‑заголовками (что и где лучше отдавать)?</summary>

  Политики безопасности и кеширования (CSP, cache headers, permissions) обычно лучше отдавать через HTTP‑заголовки; meta‑теги подходят для описательных целей и как fallback.

</details>

<details>
  <summary>42. Что такое Critical Rendering Path и какие HTML‑практики его оптимизируют?</summary>

  Critical Rendering Path — последовательность шагов от получения HTML до отображения; оптимизации: минимизировать render‑blocking ресурсов, inline критический CSS, `defer`, `preload`.

</details>

<details>
  <summary>43. Что такое SRI (Subresource Integrity) и как применять для внешних скриптов/стилей?</summary>

  SRI использует атрибут `integrity` с хэшем ресурса, чтобы браузер отверг изменённый CDN‑ресурс; применяется вместе с `crossorigin`.

</details>

<details>
  <summary>44. Как HTML взаимодействует с internationalization (hreflang, lang, dir)?</summary>

  `lang` и `dir` помогают поисковикам и вспомогательным технологиям; `hreflang` в `<link>` указывает языковые/региональные версии страниц.

</details>

<details>
  <summary>45. Какие rel‑типы ссылок важно знать (stylesheet, icon, manifest, canonical, alternate)?</summary>

  Частые `rel`: `stylesheet`, `icon`/`shortcut icon`, `manifest`, `canonical`, `alternate`, `preload`, `prefetch`, `preconnect`.

</details>

<details>
  <summary>46. Server‑side rendering (SSR) vs client‑side rendering (CSR) — как это связано с HTML?</summary>

  SSR отдаёт готовый HTML с сервера (лучше для SEO и первого рендера); CSR отдаёт минимальный HTML и рендерит на клиенте с помощью JS. Выбор зависит от требований к SEO, производительности и UX.

</details>

<details>
  <summary>47. Какие ещё meta‑теги важно упомянуть для безопасности и приватности?</summary>

  Упомянуть: `Content-Security-Policy` (лучше в заголовке), `referrer`/`referrer-policy`, `permissions-policy` (Feature-Policy). Эти политики чаще выставляют через HTTP.

</details>