# xfitter_install_docker
Install xfitter using docker image


## Step 1. Install Docker and git
```
brew install --cask docker
brew install git
```

## Step 2. Clone the repository to the path you want
```
git clone https://gitlab.cern.ch/fitters/xfitter.git
cd xfitter
```

## Step 3. Replace the Dockerfile with the one in this repository

in the xfitter folder that you just cloned, there is a Dockerfile, replace it with the Dockerfile_xfitter in this repository

```
rm Dockerfile
cp /path/to/this/repository/Dockerfile_xfitter ./Dockerfile
```

## Step 4. Build the docker image

build an image named xfitter_image
```
docker build -t xfitter_image .
```

if you are using M1 mac, you need to build the image with the following command
```
docker buildx create --use
docker buildx build --platform linux/amd64 -t xfitter_image .
```

## Step 5. Run the docker image in terminal
```
docker run -it --name xfitter_container xfitter_image /bin/bash
```
