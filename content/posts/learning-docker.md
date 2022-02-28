---
title: "Learning Docker"
date: 2022-02-24T23:22:59+01:00
draft: true
---

- https://docker-curriculum.com/

**Userful Commands**  
- docker pull <IMAGE>
- docker images
- docker run [-it] <IMAGE>
- docker run <IMAGE> <COMMAND>
- use the `-rm` flag to delete container right after usage `docker run -rm <IMAGE> <COMMAND>`
- like unix `ps` for docker containers `docker ps [-a]`
- get help for `docker run` command `docker run --help`
- delete container to prevent eating up disk space `docker rm <CONTAINER_ID>`
    - docker rm $(docker ps -a -q -f status=exited)

## Terminology

Containers can be build using the `docker run` command from Images which can be
pulled from the Docker Hub (Images registry) with the `docker pull` command. 
List your running Containers via `docker ps`.

## Real World Docker

### Static Site Webapp

Run demo project prakhar1989/static-site from the Docker Hub with 
`docker run --rm prakhar1989/static-site`
