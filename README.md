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
* #### Клонировать репризиторий:
  ```git clone https://github.com/AlexKrup7/yamdb_final.git```
* #### Добавьте нужные Actions secrets
* #### Установите venv:
  ```python -m venv venv```
* #### Зайдите на свой сервер
* #### Остановите службу nginx:
  ```sudo systemd stop nginx```
* #### Установите docker:
  ```sudo apt install docker.io```
* #### Установите docker-compose:
  https://docs.docker.com/compose/install/
* #### Скопируйте файлы docker-compose.yaml и nginx/default.conf из вашего проекта на сервер в home/<ваш_username>/docker-compose.yaml и home/<ваш_username>/nginx/default.conf

### Автор:

 Алексей Крупин

![yamdb-workflow](https://github.com/AlexKrup7/yamdb_final/workflows/yamdb-workflow/badge.svg)