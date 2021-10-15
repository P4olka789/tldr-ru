# webpack

> Собрать файлы веб проекта: JavaScript файлы и прочие файлы ассетов в один файл.
> Подробная информация: <https://webpack.js.org>.

- Создать бандл файл из файла входной точки:

`webpack {{app.js}} {{bundle.js}}`

- Загрузить также css файлы из js файла (использует css загрузчик для `.css` файлов):

`webpack {{app.js}} {{bundle.js}} --module-bind 'css=css'`

- Собрать с переданным конфигурационным файлом (с указанным скриптом для входной точки и путём до результирующего файла) и показывать прогресс сборки:

`webpack --config {{webpack.config.js}} --progress`

- Автоматически пересобирать бандл, если были изменены файлы проекта:

`webpack --watch {{app.js}} {{bundle.js}}`