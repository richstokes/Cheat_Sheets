# Docker Cheat Sheet

### Build from dockerfile

```bash
docker build -t "simple_server:dockerfile" .
```

### Start container

```bash
docker run -p 5000:80 simple_server:dockerfile
```
_Proxies port 5000 on real system to 80 on container_

### List images

```bash
docker images
```

### List all containers

```bash
docker ps -a
```

### Kill container

```bash
docker kill 
```

### Pull latest ubuntu

```bash
docker pull ubuntu:latest
```

### Run image interactively

```bash
docker run -it ubuntu
```

### View logs

```bash
docker logs -f CONTAINER_ID
```

### View Realtime events

```bash
docker events&
```

### Run command on running container

```bash
docker exec 0bfc64488ee54d6431d43429e69b89487750809224b9324142508d7347a5f54e ls /var/www/html
```

### Delete all images and containers

```bash
docker rm $(docker ps -a -q) && docker rmi $(docker images -q)
```

### Copy files from container to host

```bash
docker cp 007713059ca4ca7524eb5e31f69b966cdbbf966d97555e67bedb42b6188ad31e:/var/www/html/foo /foo/bar/
```
