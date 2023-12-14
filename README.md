# Docker Compose Repository

![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Docker Compose](https://img.shields.io/badge/docker%20Compose-%23E60DB7ED.svg?style=for-the-badge&logo=docker&logoColor=blue)
![Redis](https://img.shields.io/badge/redis-%23DD0031.svg?&style=for-the-badge&logo=redis&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/rabbitmq-%23FF6600.svg?&style=for-the-badge&logo=rabbitmq&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-000000?style=for-the-badge&logo=nginx&logoColor=green)
![Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=for-the-badge&logo=apache-kafka&logoColor=white)

This repository contains Docker Compose configuration files for running multiple software technologies using a Docker Compose file named `software_name/docker-compose.yaml (e.g. redis/docker-compose.yaml)`.

## Usage

Clone this repository to your local machine:
```bash
git clone https://github.com/omarhosny206/docker-compose.git
```

Go inside the repo's directory:
```bash
cd docker-compose
```

Run the Docker Compose file for a specific software:
```bash
cd software_name # e.g. cd redis
# for production environment
docker-compose up -d --build
# for development environment <only if file exists>
docker-compose -f docker-compose-dev.yaml up -d --build
```

## Available images
1. **Redis** [🔗](./redis) 
    - [Production](./redis/docker-compose.yaml) (images ==> Redis)
    - [Development](./redis/docker-compose-dev.yaml) (images ==> Redis, RedisInsight v2)
2. **RabbitMQ** [🔗](./rabbitmq/docker-compose.yaml) (images ==> RabbitMQ)
3. **MySQL** [🔗](./mysql)
    - [Production](./mysql/docker-compose.yaml) (images ==> MySQL)
    - [Development](./mysql/docker-compose-dev.yaml) (images ==> MySQL, MySQL Workbench)
4. **PostgreSQL** [🔗](./postgres)
    - [Production](./postgres/docker-compose.yaml) (images ==> PostgreSQL)
    - [Development](./postgres/docker-compose-dev.yaml) (images ==> PostgreSQL, pgAdmin)
5. **MongoDB** [🔗](./mongo)
    - [Production](./mongo/docker-compose.yaml) (images ==> MongoDB)
    - [Development](./mongo/docker-compose-dev.yaml) (images ==> MongoDB, Mongo Express)
6. **NGINX** [🔗](./nginx/docker-compose.yaml) (images ==> NGINX)
7. **Kafka** [🔗](./kafka) (Kafka, ZooKeeper, Kafka-UI)
    - [Production](./kafka/docker-compose.yaml) (images ==> Kafka, ZooKeeper)
    - [Development](./kafka/docker-compose-dev.yaml) (images ==> Kafka, ZooKeeper, Kafka-UI)
