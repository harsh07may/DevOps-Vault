## Docker Images
---
Build an image from a [[Dockerfile]]
```docker
docker -t build image_name path_to_dockerfile
```

List all local images
```docker
docker images
```

Pull image from docker hub
```docker
docker pull image_name:tag
```

Remove local Image
```docker
docker rmi image_name:tag
```

Tag an Image
```docker
docker tag source_image:tag new_image:tag
```

Push Image to docker hub
```docker
docker push image_name:tag
```
## Docker Containers
---

Run Container from an image
```docker
docker run --name container_name image_name:tag
```

List all containers
```docker
docker ps -a
```
*remove -a for running*

Start/Stop/Remove a container
```docker
docker start/stop/remove container_name_or_id
```

Start a container in interactive shell mode 
```docker
docker -it run container_name_or_id sh
```

Inspect/View Logs
```docker
docker inspect/logs container_name_or_id
```

Pause/Unpause
```
docker pause/unpause container_name_or_id
```

## Volume
---
Create a volume
```docker
docker create volume volume_name
```

Start a container with a volume mapping
```docker
docker --name -v run container_name volume_name:/path/in/ container image_name:tag
```

Copy files from local fs to volume fs
```docker
docker cp local_file_or_directory container_name:/path/in/ container
```

## Network
---
List all networks and inspect
```
docker network ls
docker inspect network network_name
```

Run a container with port mapping:
```docker
docker --name -p run container_name host_port:container_port image_name
```

Create a network and connect to container
```
docker create network network_name
docker connect network network_name container_name
```