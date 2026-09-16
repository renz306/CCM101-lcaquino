# Laboratory 04 - Cloud-Native Engineer

## Mission Overview

This laboratory introduces the basic concepts of cloud-native computing through Docker. The activity covers virtualization and containers, Docker deployment, and the different stages of managing a container.

## Objectives

* Understand the basic concept of virtualization and containerization.
* Learn how Docker containers work.
* Practice using common Docker commands.
* Deploy and manage an Nginx container.
* Understand the container lifecycle.
* Develop basic skills in container management.

## Docker Deployment

### Container Management

The following Docker commands were used to manage the Nginx container.

```bash
docker ps
```

**Description:**
Shows the containers that are currently running.

```bash
docker stop nginx-server
```

**Description:**
Stops the running Nginx container.

```bash
docker ps -a
```

**Description:**
Displays all containers, including those that have already stopped.

```bash
docker rm nginx-server
```

**Description:**
Removes the stopped Nginx container from the Docker environment.

## Files Included

* `virtualization-vs-containers.md` – Comparison of virtual machines and containers.
* `docker-deployment.md` – Docker container lifecycle commands.
* `reflection.md` – Personal reflection about the laboratory activity.

## Skills Learned

* Understanding Docker containers.
* Comparing virtualization and containerization.
* Executing Docker commands in Linux.
* Managing the container lifecycle.
* Stopping, checking, and removing containers.
* Creating technical documentation using Markdown.

## Challenges Encountered

One challenge was understanding the purpose of each Docker command and how they affect a container. I also needed to distinguish between stopping and removing a container. By performing the commands step by step, I became more familiar with Docker container management and deployment.
