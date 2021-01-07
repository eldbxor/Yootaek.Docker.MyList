# Yootaek.Docker.MyList
## Mongo
docker run -d --name mongo -v ~/Workspace/docker/mongo:/data/db -p 27017:27017 mongo:4.2

## MySQL
docker run -d -p 3306:3306 -e MYSQL_ROOT_PASSWORD=mypasswd -v mysql:/root/ --name mysql mysql

## RabbitMQ
sudo docker run -d --name rabbitmq -p 5672:5672 -p 5384:15672 --restart=unless-stopped -e RABBITMQ_DEFAULT_USER=username -e RABBITMQ_DEFAULT_PASS=password rabbitmq:management
