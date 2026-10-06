# Laboratory 07 - Cloud Operations Engineer

## Mission Overview

This laboratory activity focuses on the role of a Cloud Operations Engineer in monitoring Linux host resources and containerized applications. The activity uses Linux commands and Docker tools to observe system resources, deploy an Nginx web container, generate web traffic, analyze application logs, and monitor container performance.

## Objectives

- Monitor host CPU, memory, and disk resources using Linux CLI tools.
- Deploy and monitor an Nginx web container using Docker.
- Generate successful and failed HTTP requests.
- Analyze application access logs using `docker logs`.
- Monitor container CPU and memory usage using `docker stats`.
- Document cloud operations observations using Markdown.
- Practice troubleshooting techniques used in cloud environments.

## Monitoring Commands Executed

The following commands were used during the laboratory:

```bash
free -h
df -h /
top
docker run -d --name client-website -p 8080:80 nginx
docker ps
curl http://localhost:8080
curl http://localhost:8080/hidden-admin-page
docker logs client-website
docker stats
```
## Skills Learned

Through this activity, I learned how to monitor Linux host resources, deploy a Docker container, generate and analyze HTTP traffic, inspect application logs, and monitor container CPU and memory usage. I also learned how system metrics and application logs can be used together when troubleshooting cloud-based services.
