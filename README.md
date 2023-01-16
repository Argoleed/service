# Курсовой проект
## Сервис оценки заведений
***
#### 1. Пользовательский интерфейс - https://www.figma.com/community/file/1196837811680268073
***
***
#### 2. Структура базы данных
***
#### users

| Название | Тип данных    | Описание                                          |
|----------|---------------|---------------------------------------------------|
| id       | int           | Ключевое поле                                     |
| login    | varchar(32)   | Логин                                             |
| type     | varchar(8)    | Тип пользователя (owner или visitor)              |
| hash     | text          | Хэш пароля и соли                                 |
| salt     | varbinary(16) | Соль пользователя                                 |

***
#### points
| Название | Тип данных    | Описание                                          |
|----------|---------------|---------------------------------------------------|
| id       | int           | Ключевое поле                                     |
| y        | double        | Вертикальная координата                           |
| x        | double        | Горизонтальная координата                         |
| owner    | varchar(32)   | Никнейм владельца точки                           |

***
#### information

| Название    | Тип данных    | Описание                                          |
|-------------|---------------|---------------------------------------------------|
| id          | int           | id точки                                          |
| name        | text          | Название                                          |
| description | text          | Описание                                          |
| rating      | float         | Рейтинг                                           |
| reviews     | int           | Количество отзывов                                |

***
#### reviews

| Название    | Тип данных    | Описание                                          |
|-------------|---------------|---------------------------------------------------|
| id          | int           | id точки                                          |
| username    | varchar(32)   | Никнейм посетителя                                |
| rating      | int           | Оценка посетителя                                 |
| comment     | text          | Комментарий посетителя                            |

***
***
#### 3. Алгоритмы
***
- Создание, удаление и редактирование точек (Owner)
***
![](https://github.com/Argoleed/service/blob/main/Owner.png)
***
- Создание и удаление отзывов (Visitor)
***
![](https://github.com/Argoleed/service/blob/main/Visitor.png)
***
***
#### 4. API
***

***
***
#### 5. Пользовательские сценарии работы
***
