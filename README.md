# xfitter_install_docker
Install xfitter using docker image


## Step 1. Install Docker

install Docker from the official website: https://docs.docker.com/get-docker/

do not use homebrew to install Docker (I failed to install Docker using homebrew)


## Step 2. Pull the xfitter image
```
docker pull greyyyhjc/xfitter:tutorials
```

## Step 3. Create a container from the image
```
docker run -it --name xfitter_container greyyyhjc/xfitter:tutorials /bin/bash
```

## Step 4. Get into the container

you can use vscode to connect to the container, there is an extension in the vscode called "Dev Containers", you can use it to connect to the container


## Tutorial (Thanks to Yushan for sharing the tutorial materials)

tutorial examples can be found inside the container, you can find them in the following path:
```
/home/xfitter/xFitterTutorial
```

## Note: for each example, do the following step first to link the data files
```
ln -s /home/xfitter/datafiles datafiles
```

this will create a symbolic link to the data files in the current directory, so that the example can find the data files

## Let me know if you have any questions or suggestions
```
jinchen@umd.edu
```