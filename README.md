# docker_ml
Docker for ML Practitioners Workshop

Docker commands:

## List Docker CLI commands
docker

docker container --help

## Display Docker version and info
docker --version

docker version

docker info

## Execute Docker image
docker run hello-world

## List Docker images
docker image ls

docker image ls -a

## List Docker containers (running, all)
docker container ls

docker container ls --all

## Create image using this directory's Dockerfile
docker build -t friendlyhello .  

## Run "friendlyhello" mapping port 4000 to 80
docker run -p 4000:80 friendlyhello  

## Same thing, but in detached mode
docker run -d -p 4000:80 friendlyhello

## Gracefully stop the specified container
docker container stop <hash>           
  
## Force shutdown of the specified container
docker container kill <hash>         

## Remove specified container from this machine
docker container rm <hash>        

## Remove all containers
docker container rm $(docker container ls -a -q)         

## Remove specified image from this machine
docker image rm <image id>            
  
## Remove all images from this machine
docker image rm $(docker image ls -a -q)

## Log in this CLI session using your Docker credentials
docker login             

## Tag image for upload to registry
docker tag <image> username/repository:tag  
  
## Upload tagged image to registry
docker push username/repository:tag

## Run image from a registry
docker run username/repository:tag                   

## Run image for tensorflow
docker run -it --rm -p 8888:8888 -v /path/to/code:/root/code -v /path/to/datasets:/root/data <image_name>

## Run Jupyter notebook inside container
jupyter-notebook --ip=0.0.0.0 --allow-root
