To dockerize the application

```bash
docker build -f ../src/main/deployment/Dockerfile . -t 'assignmentproxy:latest'
```

The image can be found on [dockerhub](https://hub.docker.com/r/yapilyassignment/assignmentproxy)

To run using docker compose

```bash
docker-compose -f yapily-assignment-compose.yaml up
```

Then you can use the proxy functionality

```bash
curl http://localhost:8080/positions.json?page=0
```