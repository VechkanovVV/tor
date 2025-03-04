# P2P File Sharing Application

Децентрализованное P2P-приложение для поиска и обмена файлами в локальной сети.

## Особенности
- Поиск файлов по сети с использованием TTL
- Децентрализованная архитектура
- Поддержка множества одновременных соединений
- Логирование операций в реальном времени
- Защита от цикличной пересылки запросов

## Требования
- C++17
- Boost 1.66+
- CMake 3.12+

## Доступные команды

| Команда       | Параметры               | Описание                          |
|---------------|-------------------------|-----------------------------------|
| `add_peer`    | IP:PORT                 | Добавить соседний узел            |
| `remove_peer` | IP:PORT                 | Удалить соседний узел             |
| `list_peers`  | -                       | Список подключенных узлов         |
| `add_file`    | Путь [Описание]         | Добавить файл для sharing         |
| `find_file`   | Имя файла               | Начать поиск файла                |
| `download`    | IP:PORT Хеш             | Скачать файл (в разработке)       |
| `send_message`| IP:PORT Сообщение       | Отправить текст (в разработке)    |
| `exit`        | -                       | Выход из программы                |