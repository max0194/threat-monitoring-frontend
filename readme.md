# Бэкенд приложения мониторинга ИТ-угроз

## Краткое описание приложения
Веб-приложение предназначено для отправки сотрудниками случаев возникновения ИТ-угроз в компании с указанием фактов и скриншотов угроз.

## Структура
### Стили:
- `style.css` - стили для шаблонов страниц;

### Шаблоны страниц:
- `login.html` - страница входа;
- `employee_index.html` - страница создания заявки сотрудника;
- `employee_requests.html` - страница всех заявок сотрудника;
- `specialist_index.html` - страница специалиста со всеми заявками сотрудников;
- `request.html` - страница заявки;
- `threat.html` - страница факта возникновения угрозы;
- `error.html` - страница ошибки.

### Другое:
- `pre-commit-config.yaml` - файл пре-коммита;
- `check_filenames.py` - файл проверки названий на заглавные буквы.

### Инструкция по установке и запуску:
1. Выполнить git clone https://github.com/max0194/threat-monitoring-backend.git в пустую директорию backend;
2. Выполнить git clone https://github.com/max0194/threat-monitoring-frontend.git в пустую директорию frontend;
3. Запустить контейнеры через docker compose up -d в директории /backend/compose/;
4. Выполнить команду go run ./cmd/threat-monitoring/main.go в директории backend;
5. Ввести в браузере localhost:8080.
6. Узнать необходимые данные для тестовых профилей через adminer (Адрес: localhost:8084; Сервер: threat-monitoring-db, Пользователь: postgres; Пароль: postgres; База данных: threat-monitoring);

## Стек используемых технологий:
- HTML - [Ссылка на документацию](https://developer.mozilla.org/en-US/docs/Web/HTML)
- CSS - [Ссылка на документацию](https://developer.mozilla.org/en-US/docs/Web/CSS)
- JavaScript - [Ссылка на документацию](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
