# Модальное диалоговое окно

[importance 5]

Создайте функцию `showPrompt(text, callback)`, которая выводит форму для ввода с сообщением `text` и кнопками `ОК/Отмена`.

<ul>
<li>При отправке формы (OK/ввод в текстовом поле) -- должна вызываться функция `callback` со значением поля.</li>
<li>При нажатии на `Отмена` или на клавишу [key Esc] -- должна вызываться функция `callback(null)`. Клавиша [key Esc] должна закрывать форму всегда, даже если поле для ввода сообщения не в фокусе.</li>
</ul>

Особенности реализации:
<ul>
<li>Форма должна показываться в центре окна (и оставаться в центре при изменении его размеров, а также при прокрутке окна!).</li>
<li>Текст может состоять из нескольких строк, возможен любой HTML</li>
<li>При показе формы остальные элементы страницы использовать нельзя, не работают другие кнопки и т.п, это окно -- *модальное*.</li>
<li>При показе формы -- сразу фокус на `INPUT` для ввода.</li>
<li>Нажатия [key Tab]/[key Shift+Tab] переключают в цикле только по полям формы, они не позволяют переключиться на другие элементы страницы.</li>
</ul>

Пример использования:

```js
showPrompt("Введите что-нибудь<br>... умное :)", function(value) {
  alert( value );
});
```

Демо в ифрейме:
[iframe src="solution" height=160 border=1]

Исходный HTML/CSS для формы с готовым fixed-позиционированием - в песочнице.


