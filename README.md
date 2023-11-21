# Docker Compose Repository

![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Docker Compose](https://img.shields.io/badge/docker%20Compose-%23E60DB7ED.svg?style=for-the-badge&logo=docker&logoColor=blue)
![Redis](https://img.shields.io/badge/redis-%23DD0031.svg?&style=for-the-badge&logo=redis&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/rabbitmq-%23FF6600.svg?&style=for-the-badge&logo=rabbitmq&logoColor=white)
![MySql](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)
![PostgreSql](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-000000?style=for-the-badge&logo=nginx&logoColor=green)

This repository contains Docker Compose configuration files for running multiple softwares using a Docker Compose file named `software_name.yaml (e.g. redis.yaml)`.

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
docker-compose -f software_name.yaml up -d --build
# e.g. you want to run redis: docker-compose -f redis.yaml up -d --build
```