# Cloud Deployment Engineer – Reflection

This laboratory helped me understand how containerized applications can be deployed as a complete system. Using Docker Compose, I was able to run Nextcloud and MariaDB together instead of setting up each service separately. It showed me how different components can work together to provide a functional cloud application.

I also learned that a Docker Compose file needs to be properly organized. The YAML configuration defines the services, images, ports, and environment variables required by the application. I realized that checking the configuration carefully is important because an incorrect setting can prevent the containers from starting properly.

Another useful lesson was understanding how containers communicate with each other. Nextcloud needs MariaDB to store and retrieve application data, while Docker Compose provides the network that allows the two services to communicate. This gave me a better understanding of how application and database tiers work together.

The most noticeable part of the activity was successfully opening the Nextcloud interface through the browser. Seeing the deployed application running made the commands and configuration files easier to understand because I could see the result of the deployment directly.

Overall, this laboratory improved my skills in Docker, Docker Compose, Linux commands, and cloud deployment. It also helped me understand Infrastructure as Code and how configuration files can make deployments more organized, repeatable, and easier to manage.
