---
title: "Learning Docker"
date: 2022-02-24T23:22:59+01:00
draft: true
---

- https://docker-curriculum.com/#getting-started

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

