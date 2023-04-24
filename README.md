# Useful Linux Commands

## BASH

### make a directory and cd into it
```mkdir <name> && cd $_```

### execute .sh file
```chmod +x <filename.sh>```
```./<filename.sh>```



## DOCKER

### show all docker containers 
```docker ps -a```

### stop all docker containers
```docker stop $(docker ps -a -q)```

### remove all docker containers
```docker remove -f $(docker ps -a -q)```

### remove all docker images
```docker rmi -f $(docker images -aq)```

### run a command from inside a container
```docker exec -it <container name> bash```



## NGINX

### reload nginx from inside a docker container
```docker exec -it nginx-server nginx -s reload```