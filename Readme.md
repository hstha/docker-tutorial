## Command

### run container of the img with overriding its start up command with cmd

- docker run [img] {cmd}

### list currently running docker containers

- docker ps

### list all the docker containers untill now

- docker ps --all

### remove all the cached docker imgae from local computer

- docker system prune

### stop/kill the container

#### stop gives some time to kill the command where as kill will immediately kill the process

- docker stop [container_id]
- docker kill [container_id]

### injecting cmd to currently running container

- docker exec -it [container_id] [cmd]

- docker logs [container_id]

### build the docker image

####

- docker build {-t [your-docker_id/project-name:version]} [path-to-docker-file]
