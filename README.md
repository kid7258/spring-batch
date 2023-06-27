# Docker MySQL 설치

docker run -d --name mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=1234 mysql:5.7 --character-set-server=utf8mb4 --collation-server=utf8mb4_unicode_ci

docker start mysql

docker exec -it mysql bash

mysql -u root -p

create database springbatch;

Spring batch core 아래의 경로에 해당 .sql의 내용을 수동으로 실행 가능

/org/springframework/batch/spring-batch-core/4.3.8/spring-batch-core-4.3.8.jar!/org/springframework/batch/core/schema-mysql.sql
