
## Описание
- Кастомная тема cоздана с использованием HTML, CSS и JS.
- Страница включает хедер, футер и контент на странице.
- Markdown-файлы конвертируются в HTML с помощью mkdocs.
- Автоматический деплой с помощью GitHub Actions и публикация на GitHub Pages.
- При сборке используется PostCSS с плагином cssnano.

## Установка
- Клонируйте репозиторий:  
```git clone https://github.com/<your-username>/<repository-name>.git
cd <repository-name>```

Установите Python-зависимости:  
```pip install -r requirements.txt```

Установите Node.js-зависимости:
```npm install```

Соберите минифицированный CSS:
```npm run build:css```

Запустите локальный сервер MkDocs:
```mkdocs serve```

Сайт должег быть доступен по адресу http://127.0.0.1:8000.

## GitHub Actions (workflow-yml)

Этапы пайплайна
- Checkout кода: получение всех исходников из текущего репозитория.  
- Установка Python: установка необходимой версии Python (3.x).  
- Установка зависимостей: установка всех Python-библиотек для mkdocs.  
- Сборка сайта: генерация HTML-страниц из Markdown-файлов с помощью MkDocs.  
- Деплой: автоматическая публикация содержимого папки site/ на GitHub Pages.  