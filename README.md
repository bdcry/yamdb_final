# yamdb_final

![yamdb_final workflow](https://github.com/bdcry/yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg)


Это API проекта api_yamdb, который собирает отзывы (Review) пользователей на произведения (Title). Произведения делятся на категории (Category). В каждой категории есть произведения: книги, фильмы или музыка. Произведению может быть присвоен жанр (Genres) из списка предустановленных. Новые жанры может создавать только администратор.

---

Настроен Continuous Integration и Continuous Deployment для проекта YaMDB: автоматический запуск тестов, обновление образов на Docker Hub и автоматический деплой на боевой сервер при пуше в ветку main

---

<h3> Установка и развертывание </h3>
После выполнения push необходимо зайти на сервер

    $ ssh yc-user@<IP адрес>


Выполнить миграции

    $ docker-compose exec web python manage.py migrate

Собрать статику
    
    $ docker-compose exec web python manage.py collectstatic --noinput

https://hub.docker.com/repository/docker/bdcry/yamdb_final - dockerhub
я просто не понимаю, в каком смысле "развернутый проект"?
на яндекс облаке, докерхабе или где?

http://84.252.137.219/admin/login/?next=/admin/ - облако
