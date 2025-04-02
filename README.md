# Quran WebApp 🌙1

Веб-приложение для чтения Корана с интеграцией в Telegram Mini Apps. Проект предоставляет:
- Полный текст Корана на арабском языке
- Перевод на русский язык
- Поиск по сурам
- Адаптивный интерфейс для Telegram

## 🛠 Технологии
**Frontend:**
- React 18
- React Router 6
- Telegram WebApp API
- Axios

**Backend:**
- Django 4.2
- Django REST Framework
- SQLite (для разработки)

## 🌟 Особенности
- Полная интеграция с Telegram Web Apps
- Автоматическое определение цветовой схемы Telegram
- Быстрый поиск по сурам
- Оптимизированная загрузка данных
- Поддержка навигации "Назад" в интерфейсе

## 🚀 Быстрый старт

### Требования
- Node.js 18+
- Python 3.10+
- Telegram бот с настроенным меню

### Установка
1. Клонировать репозиторий:
```bash
git clone https://github.com/Amir-Suleimanov/tg-mini-app-bot.git
```
Настроить бэкенд:

```bash
cd backend
python -m venv venv
venv/Scripts/activate
pip install -r requirements.txt
cd django
python manage.py migrate
python manage.py loaddata surahs_fixture.json
```
Запустить фронтенд:

```bash
cd frontend
npm install
npm run dev
```


🔧 Конфигурация
Переменные окружения
Создайте .env файлы для настроек:

Backend (.env):
```bash
DEBUG=True
SECRET_KEY=your-secret-key
TELEGRAM_BOT_TOKEN=your-bot-token
```

📌 Особенности реализации
Интеграция с Telegram
Использование Telegram.WebApp для нативной интеграции

Автоматическая настройка цветовой схемы

Обработка событий закрытия приложения
