<img src="docker.png" width="200"/>

[![Typing SVG](https://readme-typing-svg.herokuapp.com?size=22&color=228EE6&lines=Docker+commands)](https://git.io/typing-svg)

### Images

List all images.
```properties
docker images
```

Download image.
```properties
docker pull name_of_image:version_of_image 
```

Remove image.
```properties
docker image rm name_of_image
```

### Containers

List all running containers (with the -a parameter also lists those that are not running it).
```properties
docker ps
```

Create container with custom name (abbreviation of docker container create name_of_image).
```properties
docker create --name custom_name name_of_image
```

Remove container.
```properties
docker rm custom_name
```

Start the container.
```properties
docker start custom_name
```

Stop the container.
```properties
docker stop custom_name
```

Displays the container logs.
```properties
docker logs custom_name
```

**Docker run**

Docker run facilitates the task of initializing a container. It does the following steps:
1. It looks for a local image, if not found, it downloads it.
2. Creates the container.
3. Starts the container.
4. Show the logs.

This is the best way to do it. But, if you do not want to show the logs you should specify the -d (detached) option.

```properties
docker run --name custom_name -d name_of_image
```
