# fold

> Делает переносы строк во входном файле в соответствии с заданной шириной и печатает результат в стандартный вывод.

- Делает перенос строк для ширины по-умолчанию (80 символов):

`fold {{file}}`

- Делает переносы для ширины "30":

`fold -w30 {{file}}`

- Делает переносы для ширины "5", разбивая строку, по возможности, по пробелам:

`fold -w5 -s {{file}}`