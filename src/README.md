# Micorservices
# ArtemAdm_microservices
ArtemAdm microservices repository

# Выполнено ДЗ №1? Docker-образы Микросервисы

 - [v] Основное ДЗ
 - [] Задание со *
 - [] Задание со **

## В процессе сделано:
 - Пункт 1 // Разбить наше приложение на несколько компонентов
 - Пункт 2 // Запустить наше микросервисное приложение

##      Как запустить проект:
 - docker run -d --network=reddit --network-alias=post_db --network-alias=comment_db -v reddit_db:/data/db mongo:latest
 - docker run -d --network=reddit --network-alias=post avikss/post:1.0
 - docker run -d --network=reddit --network-alias=comment avikss/comment:1.0
 - docker run -d --network=reddit -p 9292:9292 avikss/ui:2.0

##      Как проверить работоспособность:
 docker-machine ls
 Откройте в браузере ссылку http://_ваш_IP_адрес_:9292


