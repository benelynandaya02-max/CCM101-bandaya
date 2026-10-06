# Laboratory 06 – Cloud Deployment Engineer

## Mission Overview

This laboratory focused on deploying a multi-tier private cloud storage system using Docker Compose. The application used Nextcloud as the web application and MariaDB as the database.

## Objectives

- Explain the concept of a multi-tier application architecture.
- Understand the structure of a docker-compose.yml file.
- Create a Docker Compose configuration using a Linux text editor.
- Deploy Nextcloud and MariaDB using Docker Compose.
- Access the Nextcloud web interface.
- Document Infrastructure as Code principles.

## Commands Executed

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
```

## Skills Learned

I learned how to create a Docker Compose YAML configuration and use it to deploy multiple containers. I also learned how containers communicate with each other and how Docker Compose makes multi-container deployment easier to manage.
