# HTML Forms

Ниже приведён набор вопросов и кратких ответов по теме «HTML Forms» - создание форм, свойства, валидация, доступность, безопасность и лучшие практики верстки web-форм.

---

## Вопросы:

<details>
  <summary>1. Что такое форма в HTML?</summary>

  Форма (`<form>`) — это элемент для сбора и отправки пользовательских данных на сервер. 
  Содержит поля ввода, кнопки, логические группы, элементы выбора.

</details>

<details>
  <summary>2. Какие основные элементы используются внутри формы?</summary>

  `<input>`, `<textarea>`, `<select>`, `<option>`, `<button>`, `<fieldset>`, `<legend>`, `<label>`.

</details>

<details>
  <summary>3. Какие типы input поддерживает HTML?</summary>
  
  Типы: `text`, `password`, `email`, `number`, `tel`, `date`, `checkbox`, `radio`, `file`, `range`, `search`, `color`, `submit`, `reset`, и другие.

</details>

<details>
  <summary>4. Для чего нужен атрибут action у формы?</summary>
  
  `action` указывает URL, куда будут отправлены данные формы при сабмите.
</details>

<details>
  <summary>5. Что делает атрибут method?</summary>
  
  Определяет HTTP-метод отправки данных: `GET` (по умолчанию; данные — в URL) или `POST` (данные — в теле запроса).
</details>

<details>
  <summary>6. Как работает атрибут enctype?</summary>

  Управляет форматом данных: `application/x-www-form-urlencoded` (по умолчанию), `multipart/form-data` (для загрузки файлов), `text/plain`.

</details>

<details>
  <summary>7. Как обеспечить доступность формы?</summary>

  Используйте видимые метки `<label>` для каждого поля, правильно связывайте с `for` и `id`, применяйте атрибуты `aria-*`, `role`, не забудьте о tabindex.

</details>

<details>
  <summary>8. Как работает валидация формы в HTML?</summary>
  
  Встроенные атрибуты: `required`, `pattern`, `min`, `max`, `maxlength`, `type` (например, email/number), а также кастомные сообщения через `setCustomValidity`. Можно подключать JS-валидацию.
</details>


<details>
  <summary>9. Чем client-side validation отличается от server-side?</summary>
  
  Client-side validation выполняется браузером (быстро, но можно обойти), server-side — на сервере (более безопасно и надёжно, всегда нужна для критичных данных).
</details>

<details>
  <summary>10. Зачем использовать autocomplete и как его контролировать?</summary>

  `autocomplete="on"` или `autocomplete="off"` указывает браузеру разрешить/запретить автозаполнение поля пользовательскими данными.

</details>

<details>
  <summary>11. Как используется &lt;fieldset&gt; и &lt;legend&gt;?</summary>

  `<fieldset>` группирует связанные поля, `<legend>` задаёт заголовок группы, повышая доступность и визуальное отделение.

</details>

<details>
  <summary>12. Для чего нужен атрибут novalidate?</summary>
  
  Отключает встроенную валидацию браузера для всей формы.
</details>

<details>
  <summary>13. Как безопасно обрабатывать пользовательский ввод из формы?</summary>
  
  Всегда экранируйте и валидируйте данные на сервере, чтобы предотвратить XSS, SQL-инъекции и другие атаки. Не доверяйте только валидации на клиенте.
</details>

<details>
  <summary>14. Как работает &lt;label&gt; и почему он важен?</summary>

  `<label>` связывает текст-подпись с конкретным полем ввода (через `for="id"`), обеспечивает доступность и большую зону для клика.

</details>

<details>
  <summary>15. Как реализовать форму загрузки файла?</summary>

  Используйте `<input type="file">`, у формы должен быть атрибут `enctype="multipart/form-data"`.

</details>

<details>
  <summary>16. Как реализовать переключатели (radio buttons) и флажки (checkbox)?</summary>

  Для radio: несколько `<input type="radio" name="group">` — одна из опций. Для checkbox: `<input type="checkbox">` — множественный выбор.

</details>

<details>
  <summary>17. Как управлять состоянием disabled и readonly?</summary>
  
  Атрибут `disabled` полностью отключает поле и делает его неактивным. `readonly` — поле доступно для просмотра, но нельзя менять значение.
</details>

<details>
  <summary>18. Как использовать select/option для выпадающих списков?</summary>

  `<select>` — контейнер, `<option>` — варианты выбора, `<optgroup>` — группировка. Можно задать `selected`, `disabled`.

</details>

<details>
  <summary>19. Как отправить форму по клику на Enter?</summary>

  Если есть хотя бы одно поле `<input>`, нажатие Enter спровоцирует submit формы (если нет кастомной обработки).

</details>

<details>
  <summary>20. Какие best practices для форм — UX и а11y?</summary>

  - Всегда используйте метки `<label>`
  - Группируйте поля через `<fieldset>`
  - Доступный порядок через tabindex
  - Чёткие сообщения об ошибке
  - Предупреждайте о требуемых форматах данных
  - Поддерживайте клавиатурное управление

</details>