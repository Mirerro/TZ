# TZ
Этот проект демонстрирует базовую систему DevOps для развертывания простого веб-приложения с использованием:

Docker для контейнеризации
Nginx в качестве веб-сервера
GitHub Actions для CI/CD
Docker Hub для хранения образов
Render/Heroku для развертывания (опционально)

# 1. Сборка Docker образа
docker build -t devops-webapp .

# 2. Запуск контейнера
docker run -d -p 8080:80 --name webapp devops-webapp

# 3. Открыть в браузере
open http://localhost:8080

# 1. Скачать и запустить образ из Docker Hub
docker run -d -p 8080:80 --name webapp YOUR_USERNAME/devops-webapp:latest

# 2. Открыть в браузере
open http://localhost:8080

# 1. Запуск с помощью Docker Compose
docker-compose up -d

# 2. Просмотр логов
docker-compose logs -f

# 3. Остановка
docker-compose down
