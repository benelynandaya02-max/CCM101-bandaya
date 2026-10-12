## Laboratory 08 – Cloud Security Engineer

## Mission Overview

This mission focused on securing a Linux server using the Uncomplicated Firewall (UFW). I deployed an Nginx web application, checked its availability, and configured firewall rules to allow SSH and TCP traffic on port 8080.

## Objectives

- Understand the Principle of Least Privilege and attack surface.

- Audit a running web application on a Linux server.

- Configure UFW with a Default Deny policy.

- Allow SSH and port 8080.

- Document firewall commands and security practices.

- Add evidence to my GitHub Cloud Computing portfolio.

## Commands Executed

docker run -d --name secure-web-app -p 8080:80 nginx
docker ps
curl http://localhost:8080
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
sudo ufw allow 8080/tcp
sudo ufw status numbered

## Skills Learned

I learned how to run an Nginx container, test a web application, and configure firewall rules. I also learned why SSH must be allowed before enabling a firewall and why limiting incoming connections helps improve server security.
