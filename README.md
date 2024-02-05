First install docker desktop for your distro : 

https://www.docker.com/products/docker-desktop/

Command to build the stack, will build the relevant images, in this class will only build php
$ docker compose build

Command to rebuild the stack without cache
$ docker compose build --no-cache

Command to launch the stack, -d stands for detached and lets you type commands in the terminal
$ docker compose up -d

Command to stop the stack
$ docker compose down

Command to launch a process whithin a container, it stands for interactive, lets you interact with the process in your terminal
$ docker exec -it <your container name> <the process to start>
Example for this project 
$ docker exec -it miage-php sh

Command to list all started containers
$ docker ps

Command to list all containers, included stopped ones
$ docker ps -a

Command to list all images available on the host
$ docker image ls