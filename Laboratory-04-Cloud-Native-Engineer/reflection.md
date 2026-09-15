# Reflection

This laboratory activity helped me understand the difference between a Docker container and a Virtual Machine. A Virtual Machine usually takes more time to boot because it has its own operating system and virtual hardware. In comparison, a Docker container can start within seconds because it shares the host operating system. The setup process of a container is also faster because the application can be started using a Docker image instead of installing a complete operating system.

Port mapping is necessary when running a web server inside a container because the application is running inside the container. The command `-p 8080:80` connects port 8080 of the host computer to port 80 of the container. This allows users to access the Nginx web server through `localhost:8080`. Without port mapping, the web server may not be directly accessible from the host.

When the `docker rm` command is used, the container is permanently removed. Any data stored only inside the container that is not saved using a volume or another storage method can also be lost. This shows why persistent data should be stored separately when necessary.

Containerization can improve the way software developers and IT operations teams work together. Developers can package an application and its dependencies into a container, while IT operations can deploy the same container in different environments. This supports DevOps because it makes deployment more consistent and easier to manage.

My GitHub portfolio is also evolving as I complete each laboratory activity. Laboratory 4 adds Docker, containers, Nginx deployment, and technical documentation to my previous cloud computing activities. Through these activities, I am building a more organized portfolio while improving my practical cloud computing skills.
