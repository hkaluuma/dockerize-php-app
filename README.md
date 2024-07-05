NEW COMMANDS
## Link to the video
https://www.youtube.com/watch?v=1zWFxri51qQ&t=347s

## login as a sudo user
sudo su

## install docker.io
apt install docker.io

## check if docker is installed and which version
docker --version or docker to see a bunch of staff

## install curl
apt install curl
my docker version is 24.0.7 and works with docker compose versions 2.x

## to install docker compose in linux
-DOCKER_CONFIG=${DOCKER_CONFIG:-$HOME/.docker}
-mkdir -p $DOCKER_CONFIG/cli-plugins
-curl -SL https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64 -o $DOCKER_CONFIG/cli-plugins/docker-compose

## make the binary executable
chmod +x $DOCKER_CONFIG/cli-plugins/docker-compose

## verify installation and version
docker compose version

Display: Docker Compose version v2.19.1

## git clone my project code from GitHub
https://github.com/hkaluuma/dockerize-php-app.git

## Build an image in docker
docker build -t mydemophpimage . # the . is to build the image with in this directory

## List the existing images
docker image ls #to list the image

## Search for an image if the images are many
docker image ls | grep image name #if there are many images and we want to grep out one

## to create a network
docker network create test

## to run the image
docker compose up 

docker compose up -d #to run the image in the background with out logs showing