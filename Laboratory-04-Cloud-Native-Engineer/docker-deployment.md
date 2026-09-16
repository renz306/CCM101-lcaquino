# Docker Deployment

## The Container Lifecycle

### 1. Check Running Containers

```bash
docker ps
```

This command shows the Docker containers that are currently running.

### 2. Stop the Container

```bash
docker stop nginx-server
```

This command stops the running container named `nginx-server`.

### 3. Check Container Status

```bash
docker ps -a
```

This command lists all containers, including stopped containers, to confirm that `nginx-server` has stopped.

### 4. Remove the Container

```bash
docker rm nginx-server
```

This command removes the stopped `nginx-server` container from Docker.

