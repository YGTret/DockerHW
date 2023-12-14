1.Создал два файла docker-compose(в папках dev и lab)
2.Так как сети у нас созданы из-за предыдушего задания, сразу перешёл к запуску сервисов
    docker-compose -f docker-compose.lab.yml up -d
    docker-compose -f docker-compose.dev.yml up -d
3.Проверил результаты и зафиксировал в текстовых файлах.
    docker-compose -f docker-compose.lab.yml ps
    docker-compose -f docker-compose.dev.yml ps

    docker-compose -f docker-compose.lab.yml ps > lab_results.txt
    docker-compose -f docker-compose.dev.yml ps > dev_results.txt
