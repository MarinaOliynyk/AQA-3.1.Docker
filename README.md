Шаги выполнения домашнего задания к занятию 3.1.Docker:
1. Создать локальный репозиторий с файлами (gitignore, db-api.jar, application.properties, docker-compose.yml). Инициализировать его. Сделать commit. Привязать к удаленному репозиторию на GitHub. Сделать push
2. Запустить локально PUTTY. В Session ввести выданный преподавателем ip для подключения к виртуальнотй машине Linux. Нажать Open
3. В открывшемся терминале ввести логин/пароль (выданный преподавателем)
4. Клонировать проект командой git clone https://github.com/имя_пользователя/AQA-3.1.Docker.git
5. Перейти в склонированный репозиторий: cd AQA-3.1.Docker
6. Запустить контейнеры: команда для считывания с нуля конфигурации и создания заново контейнеров (применяется если файл data уже отрабатывался ранее): docker-compose -d --force-recreate
7. Запустить SUT командой: java -jar db-api.jar (результат - Spring в терминале)
8. Открыть в браузере адрес: адрес_ip/api/cards (при установленном расширении json viewer)