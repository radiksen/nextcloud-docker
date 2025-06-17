# Nextcloud Docker — готов к запуску

Репозиторий позволяет быстро развернуть Nextcloud с базой данных MariaDB через Docker Compose.

## 🚀 Быстрый старт

```bash
git clone https://github.com/ваш-пользователь/nextcloud-docker.git
cd nextcloud-docker
cp .env.example .env
docker compose up -d
```

Открой в браузере: http://localhost:8080

## 🔧 Что внутри

- Nextcloud 28 (Apache)
- MariaDB 10.11
- Лимит загрузки файлов до 2 ГБ
- Переменные среды через .env
- Разделение томов (данные сохраняются)

## 🔐 Рекомендации

- Не загружай .env в публичный репозиторий
- Для продакшена настрой HTTPS (Nginx или Traefik)
