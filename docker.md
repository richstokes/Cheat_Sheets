# Docker Cheat Sheet

### Build from Dockerfile

```bash
docker build .
```

### Start container

```bash
docker run -p 5000:80 imagename:latest
```
_Proxies port 5000 on real system to 80 on container_

### List images

```bash
docker images
```

### List all running containers

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
docker exec CONTAINER_ID ls /var/www/html
```

### Get a bash shell on running container

```bash
docker exec -ti CONTAINER_ID /bin/bash
```

### Delete all images and containers

```bash
docker rm $(docker ps -a -q) && docker rmi $(docker images -q)
```

### Copy files from container to host

```bash
docker cp CONTAINER_ID:/var/www/html/foo /foo/bar/
```
