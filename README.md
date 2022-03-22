# docker-1

Docker-1 is a School 42 project. The purpose of this project is to study and write instructions for docker and dockerfiles.

[`docker.en.pdf`](/docker.en.pdf) is the task file.

## Usage

Install [VirtualBox](https://www.virtualbox.org/).

Install *docker* and *docker-machine*.

```shell
$ brew install docker
$ brew install docker-machine
```

## Final score

125/100 (max)

![](screenshots/score.png)

## Overview

* [**00_how_to_docker**](00_how_to_docker) - Docker commands

* [**01_dockerfiles**](01_dockerfiles)

  * [0.](01_dockerfiles/ex00/Dockerfile) Alpine image with Vim editor
  * [1.](01_dockerfiles/ex01/Dockerfile) Debian TeamSpeak server
  * [2.](01_dockerfiles/ex02/Dockerfile) Ruby container for Rails applications
  * [3.](01_dockerfiles/ex03/Dockerfile) Debian with Gitlab server (SSL and SSH)

* [**02_bonus**](02_bonus) - More Dockerfiles

  * [0.](02_bonus/c/Dockerfile) Debian with angular website
  * [1.](02_bonus/minecraft_server/start.sh) Minecraft server
