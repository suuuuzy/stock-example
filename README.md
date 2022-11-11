# stock-example

How to solve Concurrency issues
* Application Level
* Database Lock
* Redis Distributed Lock


## Settings

### MySQL
```sh
docker pull mysql
docker run -d -p 3306:3306 -e MYSQL_ROOT_PASSWORD=1234 --name mysql mysql

docker exec -it mysql bash
mysql -u root -p
create database stock_example;
use stock_example;
```

### Redis
```sh
docker pull redis
docker run --name myredis -d -p 6379:6379 redis
docker ps

docker exec -it <CONTAINER_ID> redis-cli
```


## References
* [재고시스템으로 알아보는 동시성이슈 해결방법](https://www.inflearn.com/course/%EB%8F%99%EC%8B%9C%EC%84%B1%EC%9D%B4%EC%8A%88-%EC%9E%AC%EA%B3%A0%EC%8B%9C%EC%8A%A4%ED%85%9C)
