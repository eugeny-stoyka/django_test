# Тестовая интеграция сервиса

Оригинал статьи

https://www.geeksforgeeks.org/django-sign-up-and-login-with-confirmation-email-python/

## Первая секция

### 1. Поставить необходимые зависимости
```bash
pip install -r requirements.txt
```

### 2. Создать базу данных в PostgreSql

### 3. Скорректировать настроечные файлы по пути
```bash
api/settings.py
```

### 4. Создать фиктивную почту для проверки нотификации
Так же скорректировать 
```bash
api/settings.py
```

### 5. Создать таблицы в БД
```bash
python manage.py migrate
```

### 6. Запустить вебсервер
```bash
python manage.py runserver
```

### 7. Создать пользователя и проверить аутентификацию

### Домашка
Прикрутить активацию аккаунта через почту. Поможет ссылка:
https://stackoverflow.com/questions/50298114/django-2-how-to-register-a-user-using-email-confirmation-and-cbvs

## Вторая секция

### 1. Изучить основные **git** комманды
https://proglib.io/p/git-cheatsheet

### 2. Создать новую ветку **develop** из **master**
### 3. Создать ветку **feature/email-notification**
### 4. Внести изменения из первой секции в этой ветке
### 5. Слить ветки в последовательности 
`feature/email-notification` -> `develop` -> `master`

## Третья секция

### 1. Установить postman
Попробовать авторизироваться через `GET`/`POST` запросы

### 2. Изменить токен авторизации на **JWT** взамен **CSRF**

### 3. Проделать пункт №1 еще раз

### Домашка
Создать папку `docs` и файл `README-DOCS.md`. Описать принцип работы рассмотренных токенов в новой ветке `feature/token-explaination` (создается из `develop`).

Слить в последовательности `feature/token-explaination` -> `develop` -> `master`

