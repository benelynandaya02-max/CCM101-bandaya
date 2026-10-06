# Docker Compose Guide

## What Does the Services Block Do?

The `services:` block defines the containers that make up the application. In this deployment, it contains the `database` service for MariaDB and the `app` service for Nextcloud.

## How Does Nextcloud Find the Database?

The Nextcloud application uses the `MYSQL_HOST` environment variable to identify the database service.

The value is:

```text
MYSQL_HOST=database
