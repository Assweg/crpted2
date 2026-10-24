# Учебная платформа по криптографии · Docker

![Стек](https://img.shields.io/badge/Node.js%20%C2%B7%20Express%20%C2%B7%20PostgreSQL-334155?style=flat-square) ![Семестр](https://img.shields.io/badge/семестр-4-0f766e?style=flat-square) ![Статус](https://img.shields.io/badge/статус-%D0%A3%D1%87%D0%B5%D0%B1%D0%BD%D1%8B%D0%B9%20%D0%BF%D1%80%D0%BE%D0%B5%D0%BA%D1%82-64748b?style=flat-square)

Курсовой проект на Express и PostgreSQL: учётные записи, учебные материалы и тесты. Пароли обрабатываются с помощью bcryptjs, состояние входа хранится в сессии.

## Возможности и файлы

- [server.js](server.js) — Express-приложение, регистрация, вход и маршруты учебных материалов.
- [db.js](db.js) — подключение к PostgreSQL через переменные окружения.
- [views](views/) и [public](public/) — страницы и оформление.
- [data](data/), [import_data.js](import_data.js) — учебные материалы и их импорт.

## Запуск в Docker

```bash
git clone https://github.com/Assweg/crpted2.git
cd crpted2
docker compose up --build -d
```

Приложение: `http://localhost:755`. Compose запускает PostgreSQL, приложение и сервис `seeder` для импорта данных. Схема создаётся из [db/init.sql](db/init.sql).

Остановка: `docker compose down`. Дополнительные заметки: [README_DOCKER.md](README_DOCKER.md).

## Ограничения

Проект опубликован как учебная работа. В Compose сохранены демонстрационные реквизиты и значение `SESSION_SECRET`; для внешнего стенда задайте собственные.

## Версии

[Первая итерация](https://github.com/Assweg/crpted) · [Версия с Docker](https://github.com/Assweg/crpted2) · [Курсовые материалы](https://github.com/Assweg/nstu/tree/main/3sem/%D0%9A%D1%83%D1%80%D1%81%D0%BE%D0%B2%D0%B0%D1%8F).

---

[Все учебные работы](https://github.com/Assweg/nstu) · [Профиль Assweg](https://github.com/Assweg)
