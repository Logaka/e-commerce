# E-Commerce Django Project

## Описание

Простой e-commerce сайт на Django с возможностью управления категориями и товарами через админку.

## Функциональность

- Управление товарами и категориями
- Подключение базы данных PostgreSQL
- Админ-панель Django для управления моделями
- CRUD-операции для товаров и категорий
- Загрузка и отображение изображений товаров
- Статические файлы и шаблоны с Bootstrap

---

## Установка и запуск

### 1. Клонирование репозитория

```bash
git clone https://github.com/your-repo/e-commerce.git
cd e-commerce
```

### 2. Создание и активация виртуального окружения

```bash
python -m venv .venv
source .venv/bin/activate  # macOS/Linux
.venv\Scripts\activate  # Windows
```

### 3. Установка зависимостей

```bash
pip install -r requirements.txt
```

### 4. Настройка базы данных

Открой `settings.py` и замени параметры базы данных:

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'ecom_db',
        'USER': 'postgres',
        'PASSWORD': 'your_password',
        'HOST': 'localhost',
        'PORT': '5432',
    }
}
```

### 5. Применение миграций

```bash
python manage.py makemigrations
python manage.py migrate
```

### 6. Создание суперпользователя

```bash
python manage.py createsuperuser
```

Заполни имя пользователя, email и пароль.

```
alish
password
```


### 7. Запуск сервера

```bash
python manage.py runserver
```

Проект будет доступен по адресу: [http://127.0.0.1:8000/](http://127.0.0.1:8000/)

## Доступ к админ-панели

Перейди в [http://127.0.0.1:8000/admin/](http://127.0.0.1:8000/admin/) и войди под суперпользователем.


