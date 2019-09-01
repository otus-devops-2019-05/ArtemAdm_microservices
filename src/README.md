# Micorservices
# ArtemAdm_microservices
ArtemAdm microservices repository

# Выполнено ДЗ №1? Docker:  сети, docker-compose

 - [v] Основное ДЗ
 - [] Задание со *

## В процессе сделано:
 - Пункт 1 // Работа с сетями в Docker 
 - Пункт 2 // Использование docker-compose

##      Как запустить проект:
 -- Docker network
 - docker run -d --network=front_net -p 9292:9292 --name ui avikss/ui:1.0
 - docker run -d --network=back_net --name comment avikss/comment:1.0
 - docker run -d --network=back_net --name post avikss/post:1.0
 - docker run -d --network=back_net --name mongo_db --network-alias=post_db --network-alias=comment_db mongo:latest

-- docker-compose
 - docker up -d
##      Как проверить работоспособность:
 docker-machine ls
 Откройте в браузере ссылку http://_ваш_IP_адрес_:9292

Поскольку имена контейнеров Docker должны быть уникальными, мы не можете масштабировать службу за пределами 1 контейнера,
если мы указали пользовательское имя. Попытка сделать это приводит к ошибке.
Базовое имя проекта можно сменить задав параметр:
container_name: mongo
