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
### 3. Создать ветку **feature/email-notification** от **develop**
### 4. Внести изменения из первой секции в этой ветке
### 5. Слить ветки в последовательности 
`feature/email-notification` -> `develop` -> `master`

## Третья секция

### 1. Установить postman
Попробовать авторизироваться через `GET`/`POST` запросы

### 2. Изменить токен авторизации на **JWT** взамен **CSRF**

### 3. Проделать пункт №1 еще раз (изменения не вносить в проект)

### Домашка
Создать папку `docs` и файл `README-DOCS.md`. Описать принцип работы рассмотренных токенов в новой ветке `feature/token-explaination` (создается из `develop`).

Слить в последовательности `feature/token-explaination` -> `develop` -> `master`

## Четвертая секция

### 1. Протестировать работоспособность ссылки на метод POST `/check_session/`
### 2. Создать новую ветку **feature/check_session_fix** из **develop**
### 3. Скорректировать возвращаемый результат метода в новом формате
```json
{
  "user": { "id": "foo", "name": "bar", "is_auth": false },
  "session": { "id": "python", "expire_time": "tomorrow" }
}
```
### 4. Слить в последовательности `feature/check_session_fix` -> `develop` -> `master`