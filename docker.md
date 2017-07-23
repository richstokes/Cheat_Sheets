# Docker Cheat Sheet

**Build from docker file:**

`docker build -t "simple_server:dockerfile" .`

**Start container**

`docker run -p 5000:80 simple_server:dockerfile`
(Proxies port 5000 on real system to 80 on container)

**List images**

`docker images
`

**List all containers**

`docker ps -a
`

**Kill container**

`docker kill 
`

**Pull latest ubuntu**

`Docker pull ubuntu
`

**Run image interactively**

`docker run -it ubuntu
`

**View logs**

`docker logs -f CONTAINER_ID
`


**Delete all images and containers**

`    #!/bin/bash
    # Delete all containers
    docker rm $(docker ps -a -q)
    # Delete all images
    docker rmi $(docker images -q)`
