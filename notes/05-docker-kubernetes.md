# 5. Docker and Kubernetes Basics

## Docker
- **Docker** = tool to build and run containers.
- **Dockerfile** = a recipe (text file) that says how to build an image.
- **Image** = a ready package with app + libraries. Read-only.
- **Container** = a running image.
- **Docker Hub** = online store of images.

### Example Dockerfile
```
FROM node:20-alpine
WORKDIR /app
COPY . .
RUN npm install
CMD ["node", "server.js"]
```

### Common commands
```
docker build -t myapp .        # make image
docker run -p 3000:3000 myapp  # run container
docker ps                      # list running containers
docker stop <id>               # stop
```

## Kubernetes (K8s)
- **Kubernetes** = system that runs and manages many containers automatically.
- **Pod**: smallest unit. Holds one or more containers.
- **Node**: a machine (real or virtual) that runs pods.
- **Cluster**: group of nodes.
- **Deployment**: says how many copies (replicas) of a pod to keep running.
- **Service**: gives pods a stable address.

### What Kubernetes does
Auto-restart crashed pods, scale up/down, rolling updates, load balancing.
