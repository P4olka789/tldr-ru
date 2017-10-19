# xargs

> Выполнить команду с переданными через пайп аргументами, полученные как вывод другой команды, файла или чего-то ещё.
> Вход обрабатывается как один блок текста и разбивается на отдельные аргументы по пробелам, табуляциям, переводам строк и концу файла.

- Основной способ использования:

`{{arguments_source}} | xargs {{command}}`

- Удалить все файлы с расширением `.backup`:

`{{find . -name '*.backup'}} | xargs {{rm -v}}`

- Сконвертировать переводы строк из ввода в NUL (`\0`) символ и разделить только по нему (полезно, если в вводе есть пробельные символы):

`{{arguments_source}} | tr '\n' '\0' | xargs -0 {{command}}`

- Выполнить команду по разу для каждой входной строки, заменить все вхождения шаблона (обозначен `_`) входной строкой.

`{{arguments_source}} | xargs -I _ {{command}} _ {{optional_extra_arguments}}`