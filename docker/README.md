# Test docker instalation
docker run hello-world
docker run -it ubuntu bash

# Docker commands to build and run the image
docker build -t python-app-example .
docker run -d --name python-app-container-example -p 80:80 python-app-example
docker logs python-app-container-example
docker stop python-app-container-example
docker rm python-app-container-example
docker rmi python-app-example



# UseFull docker commands
docker ps - lists all running containers
docler ps -a lists all inactive and active containers
docker images - lists all images present on your machine
docker pull {image} - pull the {image}
docker run {image} - runs the image, if it is present, if not pulls it then runs it
docker start {name/container id} - starts a container
docker attach - ataches to a container
docker logs - gets the logs from the container
docker exec - executes a command inside the container