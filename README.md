# kr2-template

Веб-приложение на Flask, хранящее счётчик обращений в Redis.

| Запрос | Ответ |
|---|---|
| GET / | увеличивает счётчик `hits`, возвращает `KR2 \| <STUDENT> \| container <id> \| hits: <n>` |
| GET /health | `ok` |
| GET /whoami | заголовки X-Forwarded-Proto, X-Real-IP, Host |

Переменные окружения: `REDIS_HOST` (localhost), `REDIS_PASSWORD`, `STUDENT` (unknown).
