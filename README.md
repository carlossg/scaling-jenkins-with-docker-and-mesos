# Scaling Jenkins with Docker and Mesos

Examples and exercises from the presentation

# Prerequisites

A recent version of [Docker](https://www.docker.com/products/overview) and [Docker Compose](https://docs.docker.com/compose/install/)

* Linux: at least Docker 1.11 and Docker Compose 1.7.1
* Mac: Docker for Mac beta, which should already include Docker Compose
* Windows: Docker for Windows beta, which should already include Docker Compose

Particularly should use Docker for Mac and Docker for Windows beta versions (not Docker Toolbox)
as they expose the Docker containers under `localhost` as the Linux version does.

All the examples are using `localhost` for a consistent experience.

Tested with Docker for Mac 1.12.0 and Docker Compose 1.8.0


After installation pull all the images using `docker-compose -f mesos-jenkins/docker-compose.yml pull`

Also pull any images you may want to use, at least

    docker pull csanchez/java-with-docker-client:8-jdk-1.12.0
    docker pull java:8-jdk
    docker pull golang:1.6
    docker pull maven:3.3.9-jdk-8
    docker pull maven:3-onbuild
