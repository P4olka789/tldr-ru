# sha256sum

> Рассчитывает криптографическую контрольную сумму по алгоритму SHA256.

- Рассчитать SHA256-сумму для файла:

`sha256sum {{файл1}}`

- Рассчитать SHA256-суммы для нескольких файлов:

`sha256sum {{файл1}} {{файл2}}`

- Прочитать файл с SHA256-суммами и проверить, что суммы для всех файлов верны:

`sha256sum -c {{файл.sha256}}`