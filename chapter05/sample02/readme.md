## Chapter 5: Engaging throttling, monitoring, and access control (sample02)

[https://github.com/microservices-security-in-action/samples/tree/master/chapter05/sample02](https://github.com/microservices-security-in-action/samples/tree/master/chapter05/sample02)

```
docker run --rm -d -p 8080:8080 --name order-processing $(docker build -q .)
docker compose -f ./monitoring/docker-compose.yml up -d

docker stop order-processing
docker compose -f ./monitoring/docker-compose.yml down
```
