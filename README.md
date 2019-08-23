# Docker Tutorial

## Installation (Ubuntu):
```
# Install Docker on Ubuntu 16.04 LTS
sudo apt-get install docker.io

# Verify Installation:
docker --version

# Run first docker image (if not present then it is downloaded and run):
sudo docker run hello-world
```

## Commands

```
sudo service docker start                           # To start the docker
sudo service docker stop                            # To stop the docker
sudo docker info                                    # Get the Information about the docker
sudo docker images                                  # List down the docker images
sudo docker ps                                      # List running containers
sudo docker ps -a                                   # List down all containers with status

sudo docker run <image_name/image_id>               # Run the docker image
sudo docker rmi <image_id>                          # Remove the docker image (-f for forcefully delete)
docker rm $(docker ps -a -q)                        # Remove all docker containers
sudo docker run -it ubuntu                          # Start linux terminal interactive mode

sudo docker start <image_id>                        # Start the container
sudo docker start <first 2-digits of container_id>  # start the container

sudo docker stats                          # Memory, CPU etc Live Usage
sudo docker system df                      # Disk Usage 
sudo docker system prun                    # Delete Non running images
sudo docker inspect <image_name/id>        # Details of Image
docker build -t my_image1:1.0 .            # Buid the image from docker file with name Dockerfile
apt install docker-compose                 # Install Docker Compose
docker-compose -v                          # Docker Compose Version
```
