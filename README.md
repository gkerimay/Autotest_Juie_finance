# QAtestingREPO


﻿# QAtestingREPO

# JUie Automated Testing Suite

**Автор:** Айгерім Бекзатова  
**Дата:** 2025-05-29

---

## 📋 Описание

Набор скриптов на Python + Selenium для автоматизации визуального и API-тестирования веб-приложения JUie ([juie.amanbay.info](https://juie.amanbay.info)).  
Цель проекта —:

- Проверка корректности рендеринга страниц «Типы аккаунтов» и «Аккаунты» в разных вьюпортах  
- Сбор скриншотов, фичей (шрифты, чекбоксы, кнопки, тексты, навигационные точки)  
- Валидация API-эндпоинтов  
- Генерация итогового отчёта в формате `.docx` или `.xlsx`

---

## 🚀 Возможности

- **Кросс-браузерная автоматизация** через Selenium WebDriver  
- **Поддержка Headed/Headless** режимов  
- **Проверка UI-стилей**: шрифты, кликабельность чекбоксов, работоспособность кнопок  
- **Скриншоты** страниц для визуального регресса  
- **API-тесты** для ключевых эндпоинтов  
- **Генерация отчёта**: Word (.docx) или Excel (.xlsx)  
- **Конфигурируемые вьюпорты** (Desktop, Tablet, Mobile)  
- **Логирование** и обработка ошибок

---

## 📦 Структура проекта

## juie-autotest/
- ** autotest.py # Основной скрипт запуска тестов
- ** report_generator.py # Модуль генерации .docx/.xlsx отчётов
- ** requirements.txt # Зависимости проекта
- ** README.md # Текущий документ
- ** screenshots/ # Папка со скриншотами после прогона

yaml
Копировать
Редактировать

---

## 🛠️ Установка

1. **Клонировать репозиторий**  
   ```bash
   git clone https://github.com/your-org/juie-autotest.git
   cd juie-autotest
Создать виртуальное окружение & установить зависимости

bash
Копировать
Редактировать
python3 -m venv .venv
source .venv/bin/activate      # Linux/macOS
.venv\Scripts\activate         # Windows
pip install -r requirements.txt
⚙️ Конфигурация
В начале autotest.py задаются основные константы:

python
Копировать
Редактировать
LOGIN_URL           = "https://juie.amanbay.info/ru/login"
ACCOUNT_TYPES_URL   = "https://juie.amanbay.info/ru/account-types"
ACCOUNTS_URL        = "https://juie.amanbay.info/ru/accounts"
LOGIN_PHONE         = "+7 777 777 77 77"
LOGIN_PASS          = "admin123"
API_ENDPOINTS       = [
    "https://juie.amanbay.info/api/account-types",
    "https://juie.amanbay.info/api/accounts"
]
VIEWPORTS           = [(1920,1080), (768,1024), (375,667)]
HEADLESS            = False      # True — без GUI, False — открывается окно
USER_AGENT          = "…"
SCREENSHOT_DIR      = "./screenshots"
REPORT_FILENAME_DOC = "test_report.docx"
REPORT_FILENAME_XLS = "account_report.xlsx"
Совет: вынести эти параметры в config.yaml или .env, если потребуется более гибкая настройка.

▶️ Запуск тестов
bash
Копировать
Редактировать
# Обычный прогон (headed)
python autotest.py

# В headless-режиме
python autotest.py --headless
По окончании будет создан:

Папка screenshots/ с визуальными снимками

Отчёт test_report.docx или account_report.xlsx в корне проекта

📄 Генерация отчёта
Word: generate_report(results, "test_report.docx")

Excel: save_to_excel(types, accounts)

Отчёт содержит:

Заголовки страниц и вьюпортов

Результаты проверок (шрифты, чекбоксы, тексты, кнопки, навигация)

Статусы API

Вставленные скриншоты

🤝 Вклад
Форкните репозиторий

Создайте свою ветку: git checkout -b feature/your-feature

Внесите изменения и протестируйте

Откройте Pull Request

Пожалуйста, следуйте принятому в проекте стилю кода и обновляйте README.md по мере расширения функциональности.

📜 Лицензия
Этот проект распространяется под MIT License.

Контакты автора:
Айгерім Ғабитқызы
✉️ gabitkyzy@gmail.com
