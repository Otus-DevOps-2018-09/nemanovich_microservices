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

### gitlab-ci
Настройка gitlab
* Поднят gitlab на vm в GCP. Добавлен docker-compose.yml для развертывания gitlab.
* Запущен gitlab-раннер на этой же машине.
* В gitlab создан проект reddit, настроен пайплайн с запуском тестов по коммиту.

### gitlab-ci-2
* Добавлены шаблоны stage и prod окружения, deploy для них "по кнопке"
 и только в тегированных ветках
* Добавлен пример динамического окружения.

### monitoring-1
* В docker-compose.yml добавлен сервис логирования prometheus
* prometheus следит за сервисами ui/post/comment + добавлен node exporter

