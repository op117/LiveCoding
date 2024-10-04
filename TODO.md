#### Автоматизация проекта 
TO DO:
1. (+) Создать проект локально 
2. (+) Создать репозиторий 
3. (+) Инициализировать репозиторий локально
4. (+) Сгенерировать ci_token в GitHub для отчетов
   - токен нужен для того чтобы с помощью config файла управлять ветками. Такой токен важно делать всегда
   - GitHub account -> Developer settings -> Personal access token -> Generate new token
   - копируем токен -> в репозиторий -> Settings -> Secrets and variables -> New repository secret
5. (+) Сделать первый коммит в origin/main
6. (+) Создать ветку gh-pages
7. (+) Убедиться в инициализации gh-pages
   - gh-pages не просто название ветки, это функционал делающий деплой на GitHub страниц
   - Для нашего проекта будем размещать Allure отчеты
   - контроль деплоя во вкладке Actions
8. (+) Построить структуру проекта
   паттерн Page Object
   base - базовые конфигурационные файлы для тестов
   config - ссылки, урлы, данные
   pages - объекты страниц 
   tests - тесты
   conftest.py -  фикстуры
   .env - логин и пароль 
9. Установка нужных зависимостей 
   pip3 install selenium pytest webdriver-manager allure-pytest
    (+) Подключить pytest
    (+) Подключить allure
   pip3 freeze > requirements.txt
   и записать все зависимости 
10. (-) Написать Dockerfile
11. (-) Написать docker-compose
12. (-) Прогнать все локально
13. (-) Написать базовый .github/workflows/config.yml
14. (-) Написать полный конфиг для хранения истории запусков