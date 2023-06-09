﻿# Useful Linux Commands

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
```docker rm -f $(docker ps -a -q)```

### remove all docker images
```docker rmi -f $(docker images -aq)```

### run a command from inside a container
```docker exec -it <container name> bash```

### build a docker image
```docker build -t <image-name> .```

### run a docker container on a network
```docker run -d --name <container-name> --network <network-name> -p 80:80 <image-to-use```



## NGINX

### reload nginx from inside a docker container
```docker exec -it nginx-server nginx -s reload```



