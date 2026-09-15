# Docker Deployment and Container Lifecycle

## Docker Commands

### 1. Pull the Nginx Image

```bash
docker pull nginx
```
### 2. Run the Nginx Container

docker run -d --name nginx-server -p 8080:80 nginx

### 3. Test the Nginx Web Server

curl http://localhost:8080

## Container Lifecycle

### 4. List Running Containers

docker ps

### 5. Stop the Container

docker stop nginx-server

### 6. Verify the Container is Stopped

docker ps -a

### 7. Remove the Container

docker rm nginx-server
