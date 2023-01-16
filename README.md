# Курсовой проект
## Сервис оценки заведений
***
#### 1. Пользовательский интерфейс - https://www.figma.com/community/file/1196837811680268073
***
***
#### 2. Структура базы данных
***
##### users

| Название | Тип данных    | Описание                                          |
|----------|---------------|---------------------------------------------------|
| id       | int           | Ключевое поле                                     |
| login    | varchar(32)   | Логин                                             |
| type     | varchar(8)    | Тип пользователя (owner или visitor)              |
| hash     | text          | Хэш пароля и соли                                 |
| salt     | varbinary(16) | Число дизлайков под постом                        |

***
##### points
