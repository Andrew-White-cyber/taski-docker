# taski-docker
О проекте:
1. Учебный проект для отработки навыков пользования docker.
2. Проект представляет из себя простой трекер задач упакованный в контейнеры.

Tech.Stack: Python, Django, DRF, Pytest, SQLite, Djoser

# Как запустить проект:

Клонировать репозиторий. В папке проекта выполнить команду:

```
docker compose -f docker-compose.local.yml up
```
В отдельном терминале применить миграции внутри контейнера:
```
docker exec taski-docker-backend-1 python manage.py migrate
```
Проект будет доступен по адресу http://localhost:8000/
