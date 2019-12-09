# Lab_4: Робота з Docker

1. Ознайомлююся з документацією `Docker`.
2. Для перевірки чи докер встановлений і працює правильно на віртуальній машині запускаю перевірку версії, виведення допомоги та тестовий імедж. Перенаправляю вивід цих команд у файл `my_work.log` та комічу його до репозиторію:
    ```
    docker -v 
    docker -h
    docker run docker/whalesay cowsay Docker is fun 
    ```
3. Ознайомлююся з документацією Dockerfile, який описує контент імеджу.
4. Для знайомства з `Docker` створюю імедж із `Django` сайтом зробленим у попередній лабораторній:

    - Використавую команди, щоб завантажити базовий імедж з репозиторію:
    ```
    docker pull python:3.7-slim
    docker images
    docker inspect python:3.7-slim
    ```
    - Створюю файл з іменем `Dockerfile` та скопіюю туди вміс з репозиторію `devops_course`;
    - Ознайомлююся із коментарями, щоб зрозуміти структуру написання `Dockerfile`;
    - Замінюю посилання на власний `Git` репозиторій із сайтом та комічу даний `Dockerfile`.