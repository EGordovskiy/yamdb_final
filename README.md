# yamdb_final
​
Учебынй проект в рамках Яндекс.Практикума.
На YaMDb читатели оставляют к произведениям текстовые отзывы и выставляют рейтинг.
​
## Требования
​
Перед запуском работы проверьте наличие 
[Python](https://www.python.org/downloads/),
[Django](https://www.djangoproject.com/), 
[Docker](https://www.docker.com/).
​
## Установка
​
*Клонируйте репозиторий на локальный компьютер. 
Выполните сборку контейнера.*
```
$ docker-compose build
```
​
*Запуск docker-compose.*
```
$ docker-compose up
```
При создании контейнера миграции выполнятся автоматически.
​
## Тестовые данные
​
*fixtures.json - используется для заполнения тестовыми данными.*
```
$ python manage.py loaddata fixtures.json
```
​
## Создание суперпользователя.
```
$ docker-compose run <CONTAINER ID> python manage.py createsuperuser
```
## Выключение контейнера.
```
docker-compose down
```
## Удаление контейнеров.
```
docker stop $(docker ps -a -q)
docker rm $(docker ps -a -q)
```
![yamdb_final workflow](https://github.com/egordovskiy/yamdb_final/workflows/yamdb_final%20workflow/badge.svg)
![yamdb_final workflow](https://github.com/egordovskiy/yamdb_final/workflows/yamdb_finalworkflow/badge.svg)
