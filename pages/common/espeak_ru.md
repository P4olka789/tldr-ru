# espeak

> С помощью синтезатора речи (TTS) говорит через звуковое устройство по-умолчанию.

- Говорит фразу вслух:

`espeak "Я люблю кататься на велосипеде."`

- Вслух читает содержимое файла:

`espeak -f {{filename}}`

- Сохраняет вывод в WAV-файл вместо произнесения вслух:

`espeak -w {{filename.wav}} "Это Линукс вместе с GNU"`

- Использует другой голос:

`espeak -v {{voice}}`