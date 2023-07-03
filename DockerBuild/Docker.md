docker stop $(docker ps -a -q)
docker rm $(docker ps -a -q)
docker rmi minhnd/base_ubuntu

COMPOSE_DOCKER_CLI_BUILD=1 docker-compose -f ./DockerBuild/docker-compose.yml build  

# Debug
docker run --rm --name base_minh -it --mount type=bind,source="$(pwd)/src/",target=/texturing/ minhnd/base_ubuntu bash

# Run example: In build dir
./apps/texrecon/texrecon ../data/apt0/apt0 ../data/apt0/apt0.ply ../result/tmp


