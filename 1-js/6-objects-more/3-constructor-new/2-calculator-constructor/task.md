# Создать Calculator при помощи конструктора

[importance 5]

Напишите *функцию-конструктор* `Calculator`, которая создает объект с тремя методами:
<ul>
<li>Метод `read()` запрашивает два значения при помощи `prompt` и запоминает их в свойствах объекта.</li>
<li>Метод `sum()` возвращает сумму запомненных свойств.</li>
<li>Метод `mul()` возвращает произведение запомненных свойств.</li>
</ul>

Пример использования:

```js
var calculator = new Calculator();
calculator.read();

alert( "Сумма=" + calculator.sum() );
alert( "Произведение=" + calculator.mul() );
```

[demo /]
