# Laboratory 10: Enterprise Cloud Architect

## Mission Overview

This mission focuses on designing, deploying, securing, and documenting an enterprise cloud infrastructure. The proposed project uses Ubuntu Server, Docker Compose, Nextcloud, and MariaDB to create a multi-tier application environment.

## Objectives

- Design a network topology and cloud architecture diagram.
- Install and configure Ubuntu Server in a virtual machine.
- Install Docker and Docker Compose.
- Deploy Nextcloud and MariaDB using Docker Compose.
- Configure persistent storage so application and database data can survive container restarts.
- Secure the server using UFW and a default-deny incoming policy.
- Create a Bash script for automated backups and schedule it using cron.
- Document deployment, security, maintenance, and recovery procedures.
- Reflect on the knowledge gained from Laboratory Activities 1 through 10.

## Project Architecture

The proposed architecture consists of a host computer, a hypervisor, an Ubuntu Server virtual machine, a host-based firewall, and two linked containers. Nextcloud provides the web application, while MariaDB stores the application's database information. Persistent volumes are used to retain data.

## Main Components

- **Ubuntu Server:** Hosts and manages the application environment.
- **Docker Engine:** Runs the application containers.
- **Docker Compose:** Defines and manages the multi-container application.
- **Nextcloud:** Provides web-based file management.
- **MariaDB:** Provides database services for Nextcloud.
- **UFW:** Controls incoming and outgoing network traffic.
- **Bash and cron:** Automate operational tasks such as scheduled backups.

## Security and Data Protection

The server will use a default-deny incoming firewall policy and allow only the ports required for remote administration and web access. The database should remain on the internal Docker network and should not be exposed directly to the host network. Persistent volumes and scheduled backups will support data protection and recovery.

## Commands Executed

This section will be updated with the commands actually used during installation, deployment, security configuration, and testing.

## Testing and Evidence

The completed project will include an architecture diagram and evidence of the running application, firewall configuration, persistent storage, and backup automation. Only tests that have been performed successfully will be reported as completed.

## Skills Learned

This project provides an opportunity to practice virtual machine setup, Linux administration, container deployment, network security, persistent storage, Bash scripting, cron scheduling, technical documentation, and cloud infrastructure planning.
