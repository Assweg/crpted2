# crpted2 — Курсовая: веб-приложение с авторизацией (v2, Docker)

Вторая итерация курсового проекта, 4 семестр. Всё то же, что в `crpted`, но с Docker-окружением.

## Отличия от v1
- Добавлены `Dockerfile`, `docker-compose.yml`, `.dockerignore`
- `README_DOCKER.md`, скрипты `npm run build/up/down`
- Зависимости: + `dotenv`, `connect-pg-simple`, `chart.js`, `csurf`

## Стек
Node.js, Express, PostgreSQL, Docker Compose

## Запуск
```bash
npm install
docker-compose up --build
# или локально:
npm start
```

## Что изучено
Контейнеризация Node.js + Postgres, переменные окружения, хранение сессий в БД.

---
**Автор:** Assweg · Telegram: [@assweg](https://t.me/assweg) · Учебное портфолио, все работы — студенческие.
