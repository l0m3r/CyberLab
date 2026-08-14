
# 📄 Cheatsheet: [curl]
> популярная утилита командной строки для передачи данных на сервер и с сервера по множеству протоколов (включая HTTP, HTTPS, FTP).


## 📋 Основные команды
| Команда | Описание | Пример |
|---------|----------|--------|
| `curl <URL>` | Выполнить GET-запрос к указанному URL | `curl http://example.com/` |
| `curl -X <METHOD> <URL>` | Указать HTTP-метод (GET, POST, PUT, DELETE и т.д.) | `curl -X POST http://example.com/api` |
| `curl -d "data" <URL>` | Отправить данные в теле запроса (метод POST по умолчанию) | `curl -d "name=John&age=30" http://example.com/form` |
| `curl -d "param1=val1" -d "param2=val2" <URL>` | Передать несколько параметров через несколько `-d` | `curl -d "want_flag=YES" -d "code=1337" http://example.com/` |
| `curl --data-urlencode "data" <URL>` | URL-кодировать данные перед отправкой (полезно для пробелов и спецсимволов) | `curl --data-urlencode "fun=Kaspersky & Summer & Lab" http://example.com/` |
| `curl -H "Header: value" <URL>` | Добавить произвольный заголовок в запрос | `curl -H "SPbCTF: Pretty cool" http://example.com/` |
| `curl -H "Cookie: name=value" <URL>` | Установить Cookie-заголовок (или использовать `-b`) | `curl -H "Cookie: session=abc123" http://example.com/` |
| `curl -b "Cookie: name=value" <URL>` | Отправить Cookie (альтернатива `-H "Cookie: ..."`) | `curl -b "Cookie: id=1" http://example.com/` |
| `curl -c <файл> <URL>` | Сохранить полученные Cookie в файл (в формате Netscape) | `curl -c cookies.txt http://example.com/` |
| `curl -b <файл> <URL>` | Использовать Cookie из файла при запросе | `curl -b cookies.txt http://example.com/` |
| `curl -v <URL>` | Включить подробный вывод (verbose) — показывает заголовки запроса и ответа | `curl -v http://example.com/` |
| `curl -h` или `curl --help` | Показать краткую справку по командам curl | `curl --help` |
| `curl --help all` | Показать полную справку по всем опциям | `curl --help all` |


## 📚 Полезные ресурсы
- https://curl.se/
