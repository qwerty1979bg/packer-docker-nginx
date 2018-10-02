# Packer template to create an NGINX docker image 

This repository contains a Packer template for building an NGINX docker image

## Usage

1. [Install Packer](https://www.packer.io/intro/getting-started/install.html#precompiled-binaries)
2. [Install Docker](https://docs.docker.com/install/#supported-platforms)
3. Clone this repository and `cd` into it.

4. Run the following:

```
$ export DOCKER_HUB_USERNAME=<Your Docker HUB username>
$ export DOCKER_HUB_PASSWORD=<Your Docker HUB password>
$ packer build docker-nginx.json
```

5. The image should be pushed to the Docker HUB

## To use the box with Docker Hub:

```
$ docker pull <USERNAME>/test-nginx
```
