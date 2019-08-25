# ArtemAdm_microservices
ArtemAdm microservices repository

# Выполнено ДЗ №1? Технология контейнеризации. Введение в Docker

 - [v] Основное ДЗ
 - [v] Задание со *
 - [] Задание со **

## В процессе сделано:
 - Пункт 1 // Создание docker host
 - Пункт 2 // Создание своего образа
 - Пункт 3 // Работа с Docker Hub

##      Как запустить проект:
 - docker run --name reddit -d --network=host reddit:latest
 - 

##      Как проверить работоспособность:
 docker-machine ls
 Откройте в браузере ссылку http://_ваш_IP_адрес_:9292

 docker run --name reddit -d -p 9292:9292 <your-login>/otus-reddit:1.0

