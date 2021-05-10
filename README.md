# matveevelli_microservices

###Домашняя работа №15

- Создана ВМ я yc с докер-хост
- Добавлены каталоги из архива reddit-microservices
- Созданы dockerfile для микросервисов
- Создана docker-bridge сеть
- Запущены контейнеры и проверена работоспособность
- Переименованы сетевые алиасы на reddit_post и reddit_comment, переопределение происходит через ENV переменные в docker run `docker run -d --network=reddit -p 9292:9292 --env POST_SERVICE_HOST=reddit_post --env COMMENT_SERVICE_HOST=reddit_comment matveevelli/ui:5.0`
- Улучшен образ микросервиса на основе alpine, 265MB
- Создан volume для mongodb

###Домашняя работа №14

- Установил docker, docker-compose, docker-machine
- Запустил первый контейнер
- Сохранил вывод команды docker images в файл dockermonolith/docker-1.log
- Сравнил вывод команд docker inspect <u_container_id> и docker inspect <u_image_id> и записали в файл - docker-1.log
- Инициализировал хост docker-machine в Yandex Cloud
- Собрали образ с приложением с помощью файлов Dockerfile, db_config, start.sh, mongod.conf
- Запустили контейнер, проверили результат работы приложения
- Зарегистрировался на Docker hub и запушил туда image
- Поигрался с "проверочными" командами
