# Reflection

## 1. Docker Compose and Cloud Engineering

Writing a `docker-compose.yml` file made the deployment easier because I only needed to define the containers, images, ports, and environment variables in one file. Instead of typing many commands one by one, I could use `docker-compose up -d` to deploy the whole application. This makes the deployment faster, more organized, and easier to repeat.

## 2. YAML Indentation

I learned that YAML is sensitive to indentation. If I use a Tab instead of Spaces or place an item at the wrong level, the Compose file may show an error and the deployment may not work. This taught me to be careful with spacing and to follow the correct structure when writing YAML configuration files.

## 3. Environment Variables

Environment variables such as `MYSQL_PASSWORD` are used to provide configuration values to the containers. They allow the Nextcloud application and MariaDB database to use the required settings, such as the database name, username, and password. I learned that these variables help containers communicate and work together correctly.

## 4. Deploying Nextcloud

When I accessed the Nextcloud setup page, I felt happy because I was able to see a real cloud storage application running from the containers I deployed. It was also interesting to see how Docker Compose connected Nextcloud with the MariaDB database. This activity helped me understand how cloud applications can be deployed.

## 5. My Cloud Computing Progress

Since Mission 1, my understanding of Cloud Computing has changed because I now understand more about how cloud infrastructure works. I learned about Linux commands, cloud infrastructure, containers, storage, and multi-container applications. Before, I mostly understood cloud computing as online storage and services. Now, I understand that cloud computing also involves deploying, managing, connecting, and documenting different services.
