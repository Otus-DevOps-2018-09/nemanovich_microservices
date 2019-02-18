# nemanovich_microservices
nemanovich microservices repository

### docker-2

Настройка докера для монолитного приложения
* Добавлен Dockerfile для запуска приложения reddit
* Image опубликован в docker-hub:
 https://cloud.docker.com/u/otusstudy/repository/docker/otusstudy/otus-reddit

### docker-3
Настройка докера для микросервисного приложения
* Добавлены Dockerfile's для микросервисов reddit

### docker-4
Настройка docker-compose
* Добавлен docker-compose для деплоя reddit (фронт и бд расположены в разных сетях)
* Для изменения префикса запускаемых контейнеров
можно использовать опцию -p: `docker-compose -p MY_PROJECT_NAME up`
