
# Docker Commands Reference

## Image Management

Build an image:

```bash
docker build -t my-docker-app:v1 .
```

List images:

```bash
docker images
```

Remove an image:

```bash
docker rmi IMAGE_NAME
```

## Container Management

List running containers:

```bash
docker ps
```

List all containers:

```bash
docker ps -a
```

Stop a container:

```bash
docker stop web-container-1
```

Start a container:

```bash
docker start web-container-1
```

Restart a container:

```bash
docker restart web-container-1
```

View logs:

```bash
docker logs web-container-1
```

## Docker Compose

Start services:

```bash
docker compose up -d
```

Stop services:

```bash
docker compose down
```

Rebuild services:

```bash
docker compose up -d --build
```

View services:

```bash
docker compose ps
```

## Cleanup

Check disk usage:

```bash
docker system df
```

Remove unused images:

```bash
docker image prune
```

Remove stopped containers:

```bash
docker container prune
```
