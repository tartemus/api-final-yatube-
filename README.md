# API для Yatube

## Описание
Проект предоставляет API для социальной сети **Yatube**.  
Через API можно:
- создавать и редактировать посты,
- просматривать группы,
- подписываться на других пользователей,
- оставлять комментарии к постам.

Документация доступна по адресу:  
`http://127.0.0.1:8000/redoc/`

## Установка и запуск
1. Клонируйте репозиторий:
   ```bash
   git clone <ссылка-на-репозиторий>
   cd api_final_yatube

2. Установите и активируйте виртуальное окружение:

python -m venv venv
source venv/bin/activate   # Linux/MacOS
venv\Scripts\activate      # Windows

3. Установите зависимости:

pip install -r requirements.txt

4. Выполните миграции:

python manage.py migrate

5. Запустите сервер разработки:

python manage.py runserver


Получение всех постов:
GET /api/v1/posts/

Создание поста:
POST /api/v1/posts/

{
  "text": "Новый пост через API"
}