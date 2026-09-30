# Docker Compose Guide – Nextcloud Cloud Deployment

This guide describes how Docker Compose is used to run a Nextcloud application together with a MariaDB database. The two services work together to provide the complete cloud storage environment.

## Understanding the Compose File

The `docker-compose.yml` file contains the configuration needed for the deployment. Under the `services:` section, each application component is defined separately.

The main services are:

- **database** – Runs MariaDB and handles database storage.
- **app** – Runs Nextcloud and provides the web interface.

Each service can have settings such as its Docker image, environment variables, ports, and other configuration options.

## How Nextcloud Connects to MariaDB

Nextcloud uses the database service name to communicate with MariaDB.

For example:

```text
MYSQL_HOST=database
