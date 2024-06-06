# xfitter_install_docker
Install xfitter using docker image


## Step 1. Install Docker

install Docker from the official website: https://docs.docker.com/get-docker/

do not use homebrew to install Docker (I failed to install Docker using homebrew)


## Step 2. Pull the xfitter image
```
docker pull greyyyhjc/xfitter:camp
```

## Step 3. Create a container from the image
```
docker run -it --name xfitter_container greyyyhjc/xfitter:camp /bin/bash
```

## Step 4. Get into the container

you can use vscode to connect to the container, there is an extension in the vscode called "Dev Containers", you can use it to connect to the container


## Tutorial

tutorial examples can be found at https://www.xfitter.org/xFitter/tutorials
