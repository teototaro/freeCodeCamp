---
title: Python Truth Value Testing
localeTitle: Тестирование ценности правды Python
---
[Документы Python - проверка истины](https://docs.python.org/3/library/stdtypes.html#truth-value-testing)

Любой объект может быть проверен на значение истины, для использования в `if` или `while` или в качестве операнда логической операции типа `and` , `or` , или `not` .

Следующие значения считаются ложными:

*   `None`
*   `False`
*   ноль любого числового типа, например, `0` , `0.0` , `0j` , `Decimal(0)` , `Fraction(0, 1)` .
*   любая пустая последовательность, например, `''` , `()` , `[]` , `set()` , `range(0)` .
*   любое пустое отображение, например `{}` .
*   экземпляры пользовательских классов, если класс определяет `__bool__()` или `__len__()` , когда этот метод возвращает `False` или `0` .

Все остальные значения считаются истинными, поэтому объекты многих типов всегда верны.

Операции и встроенные функции, которые имеют логический результат, всегда возвращают `0` или `False` для false и `1` или `True` для true, если не указано иное. (Важное исключение: логические операции `or` `and` всегда `and` всегда возвращают один из их операндов.)