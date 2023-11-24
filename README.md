# Тестовая интеграция сервиса

Оригинал статьи

https://www.geeksforgeeks.org/django-sign-up-and-login-with-confirmation-email-python/

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

### 5. Создать пользователя и проверить аутентификацию

### Домашка
Прикрутить активацию аккаунта через почту. Поможет ссылка:
https://stackoverflow.com/questions/50298114/django-2-how-to-register-a-user-using-email-confirmation-and-cbvs