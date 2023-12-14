
1.Создал файл docker-compose.yml(Файл прилагаю)
2.Дальше создал сети:
    docker network create dev_network
    docker network create prod_network
    docker network create lab_network
3.Запустил сервисы:
    docker-compose -f docker-compose.yml -p dev up -d
    docker-compose -f docker-compose.yml -p prod up -d
    docker-compose -f docker-compose.yml -p lab up -d
4.Далее посмотрел все заущенные контейнеры(SS1)  
    docker ps
5.Посмотрел статус всех сервисов в окружениях(SS1):
    docker-compose -f docker-compose.yml -p dev ps
    docker-compose -f docker-compose.yml -p prod ps
    docker-compose -f docker-compose.yml -p lab ps
