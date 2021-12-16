# Проект api_YaMDb

## Описание

#### Устанавливается из контейнера Docker

#### Проект YaMDb собирает отзывы пользователей на произведения

#### Произведения делятся на категории(например, "Музыка", "Фильмы" и тд.)

#### Каждому произведению может быть присвоен жанр(например, "Роман", "Поп" и тд.)

#### Новые жанры может создавать только администратор

### Пример

* Музыка
    * Поп
        * Позови меня с собой-Алла Пугачёва
        * Он тебя целует-Руки Вверх

    * Рок
        * Highway To Hell-AC/DC
        * The Unforgiven-Metallica
* Фильмы
    * Ужасы
        * Пятница 13
        * Пила
    * Комедии
        * Американский пирог
        * ДМБ
## Обратная связь
#### Пользователи могут оставить к произведениям отзывы, а так же оценку
#### На одно произведение пользователь может оставить только один отзыв
#### Благодаря оценкам пользователей формируется рейтинг
## Установка:

* Установка docker:
https://www.docker.com/products/docker-desktop

* Создать файл .env с переменными окружения:
```
DB_ENGINE=django.db.backends.postgresql
DB_NAME=postgres # Имя базы данных
POSTGRES_USER=postgres # Администратор базы данных
POSTGRES_PASSWORD=postgres # Пароль администратора
DB_HOST=db
DB_PORT=5432
```
*  Сборка и запуск контейнера
```docker-compose up -d --build```
   
* Сбор статики
```docker-compose exec web python manage.py collectstatic --noinput```
  
* Создание суперпользователя
```docker-compose exec web python manage.py createsuperuser```
#### Адрес сервера

http://127.0.0.1:8000/

#### Документация

http://127.0.0.1:8000/redoc/

### Автор:

 Алексей Крупин

![yamdb-workflow](https://github.com/AlexKrup7/yamdb_final/workflows/yamdb-workflow/badge.svg)