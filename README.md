# yamdb_final

![yamdb_final workflow](https://github.com/bdcry/yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg)

<<<<<<< HEAD
Это API проекта api_yamdb, который собирает отзывы (Review) пользователей на произведения (Title). Произведения делятся на категории (Category). В каждой категории есть произведения: книги, фильмы или музыка. Произведению может быть присвоен жанр (Genres) из списка предустановленных. Новые жанры может создавать только администратор.

---

Настроен Continuous Integration и Continuous Deployment для проекта YaMDB: автоматический запуск тестов, обновление образов на Docker Hub и автоматический деплой на боевой сервер при пуше в ветку main

---

<h3> Установка и развертывание </h3>
После выполнения push необходимо зайти на сервер

    $ ssh yc-user@<IP адрес>

Перейти в директорию app

    $ cd app/

Выполнить миграции

    $ docker-compose exec web python manage.py migrate

Собрать статику
    
    $ docker-compose exec web python manage.py collectstatic --noinput
=======
![yamdb_final workflow](https://github.com/bdcry/yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg)
>>>>>>> da5c31281f3082193127386fdc478f246ec9c1fa
