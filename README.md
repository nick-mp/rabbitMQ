# Домашнее задание к занятию "Очереди RabbitMQ" - Горегляд Николай

### Задание 1. Установка RabbitMQ

`Используя Vagrant или VirtualBox, создайте виртуальную машину и установите RabbitMQ. Добавьте management plug-in и зайдите в веб-интерфейс.`
`Итогом выполнения домашнего задания будет приложенный скриншот веб-интерфейса RabbitMQ`

##### ответ:
 ![Task1](https://github.com/nick-mp/rabbitMQ/blob/main/img/install_rabbitmq.png)
 ![Task1-2](https://github.com/nick-mp/rabbitMQ/blob/main/img/2_1_add_queues.png)

### Задание 2. Отправка и получение сообщений

`Используя приложенные скрипты, проведите тестовую отправку и получение сообщения. Для отправки сообщений необходимо запустить скрипт producer.py.`
`Для работы скриптов вам необходимо установить Python версии 3 и библиотеку Pika. Также в скриптах нужно указать IP-адрес машины, на которой запущен RabbitMQ, заменив localhost на нужный IP.`
`Зайдите в веб-интерфейс, найдите очередь под названием hello и сделайте скриншот. После чего запустите второй скрипт consumer.py и сделайте скриншот результата выполнения скрипта`
`В качестве решения домашнего задания приложите оба скриншота, сделанных на этапе выполнения.`

##### ответ:
 ![Task2](https://github.com/nick-mp/rabbitMQ/blob/main/img/3_1_start_consumer.png)
 ![Task2-1](https://github.com/nick-mp/rabbitMQ/blob/main/img/3_2_start_Produser.png)

### Задание 3. Подготовка HA кластера

`Используя Vagrant или VirtualBox, создайте вторую виртуальную машину и установите RabbitMQ. Добавьте в файл hosts название и IP-адрес каждой машины, чтобы машины могли видеть друг друга по имени.`
`Затем объедините две машины в кластер и создайте политику ha-all на все очереди.`
`Также приложите вывод команды с двух нод:`
 ![Task_3-1](https://github.com/nick-mp/rabbitMQ/blob/main/img/4_1_rbm1_cluster_status.png)
 ![Task_3-2](https://github.com/nick-mp/rabbitMQ/blob/main/img/4_1_rbm2_cluster_status.png)

`Для закрепления материала снова запустите скрипт producer.py и приложите скриншот выполнения команды на каждой из нод:`
`rabbitmqadmin get queue="hello"`
`Приложите скриншот результата работы второго скрипта.`

 ![Task_3-3](https://github.com/nick-mp/rabbitMQ/blob/main/img/4_2_script.png)
 `на графике видны все отправленные сообщения`