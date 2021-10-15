# runcon

> Запускает программу в другом контексте безопасности SELinux.
> Не используя ни контекста, ни команды, выводит текущий контекст безопасности.


- Определить текущий домен:

`runcon`

- Указать домен для запуска команды:

`runcon -t {{domain}}_t {{command}}`

- Указать роль контекста для запуска команды с ним:

`runcon -r {{role}}_r {{command}}`

- Указать полный контекст для запуска команды:

`runcon {{user}}_u:{{role}}_r:{{domain}}_t {{command}}`