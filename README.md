NEW COMMANDS
## Link to the video
https://www.youtube.com/watch?v=1zWFxri51qQ&t=347s

## login as a sudo user
sudo su

## Install docker.iogit
apt install docker.io

## Check if docker is installed and which version
docker --version : to see the docker version.
docker to see a bunch of staff

my docker version is 24.0.7 and works with docker compose versions 2.x

## Install curl
apt install curl

## to install docker compose in linux
DOCKER_CONFIG=${DOCKER_CONFIG:-$HOME/.docker}

mkdir -p $DOCKER_CONFIG/cli-plugins

curl -SL https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64 -o $DOCKER_CONFIG/cli-plugins/docker-compose

## Make the binary executable
chmod +x $DOCKER_CONFIG/cli-plugins/docker-compose

## Verify installation and version
docker compose version

Display: Docker Compose version v2.19.1

## To clone my project code from GitHub
https://github.com/hkaluuma/dockerize-php-app.git

## Change Directory to the folder of the project where there is the docker compose.yml file
cd Dockerize-PHP-Application

## Build an image in docker
docker build -t mydemophpimage . # the . is to build the image with in this directory

## List the existing images
docker image ls #to list the image

## Search for an image if the images are many
docker image ls | grep image name #if there are many images and we want to grep out one

## To create a network
docker network create test

## To list existing networks to see if the new one is there
docker network ls

## To run the image
docker compose up 

docker compose up -d #to run the image in the background with out logs showing

## Other common commands of docker you may need inlude:
### to list the containers
docker ps -a 
### to remove the docker container
docker rm 0ea91f8511d4 # where 0ea91f8511d4 is the container id
### to list the docker images
docker image list
### to list the containers
docker rmi rmi 4a6df810d2c4 # where 4a6df810d2c4 is the image id
