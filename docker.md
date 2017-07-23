# Docker Cheat Sheet

**Build from dockerfile**

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

**Run command on running container**

`docker exec 0bfc64488ee54d6431d43429e69b89487750809224b9324142508d7347a5f54e ls /var/www/html`


**Delete all images and containers**

`docker rm $(docker ps -a -q) && docker rmi $(docker images -q)
`
