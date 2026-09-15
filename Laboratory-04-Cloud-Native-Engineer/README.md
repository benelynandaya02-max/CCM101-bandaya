# Laboratory Activity 4: The Cloud-Native Engineer

## Mission Overview

This laboratory activity focuses on understanding the difference between Virtual Machines and Containers. It also introduces Docker commands and the deployment of an Nginx web server using a container. Using the KillerCoda Playground, I learned how to verify Docker, pull an Nginx image, run a container, test the web server, and manage the container lifecycle.

## Objectives

- Differentiate between Virtual Machine and Containers.
- Access a Docker-enabled cloud environment using KillerCoda.
- Execute fundamental Docker CLI (Command Line Interface) commands.
- Pull, run, manage and terminate a containerized application (Nginx).
- Create professional technical documentation of container operations using Markdown.
- Continue developing a well-organized GitHub Cloud Computing Portfolio.

## Docker Commands Executed

### Checkpoint 3 - Enter the Docker Playground

I used the following commands to verify the Docker was installed and running:

```bash
docker --version
docker info
```
## Checkpoint 4 - Pull and Run Nginx

I pulled the Nginx image from Docker Hub and launched it as a container:

docker pull nginx
docker run -d --name nginx-server -p 8080:80 nginx

## Checkpoint 5 - Test and Manage the Container

I used the following commands to check and test the running Nginx container:

docker ps
curl http://localhost:8080
docker logs nginx-server

I also stopped, checked, and removed the container:

docker stop nginx-server
docker ps
docker rm nginx-server

## Skills Learned

I learned how to compare Virtual Machines and Containers and use basic Docker commands. I also learned how to run an Nginx container, map ports, test a web server, and manage Docker containers.

## Challenges Encountered

I had difficulty understanding Docker commands, port mapping, and container management. I also encountered a Git author identity error, which I solved by configuring my Git username and email.

## Conclusion

This activity helped me understand containers, Docker, and how they differ from Virtual Machines. It also improved my skills in Docker, cloud computing, Markdown, and GitHub.

