# Laboratory 06 – Cloud Deployment Engineer

## Mission Overview

This laboratory demonstrates how to deploy a cloud-based file storage system using Docker Compose. The setup uses Nextcloud as the application service and MariaDB as its database. Docker Compose allows both containers to be configured and launched as one deployment.

## Learning Goals

- Build a simple multi-container cloud environment.
- Configure services using Docker Compose.
- Connect Nextcloud with a MariaDB database.
- Deploy and manage containers through Docker commands.
- Access the application using a mapped port.
- Apply Infrastructure as Code principles.

## Deployment Commands

| Command | Description |
|---|---|
| `mkdir nextcloud-deployment` | Creates the workspace for the deployment. |
| `cd nextcloud-deployment` | Opens the project directory. |
| `nano docker-compose.yml` | Creates the Docker Compose configuration. |
| `cat docker-compose.yml` | Views the Compose configuration. |
| `docker compose up -d` | Starts the required containers. |
| `docker compose ps` | Displays the running container status. |
| `docker compose down` | Stops and removes the deployed services. |

## Architecture

The deployment consists of two main services:

- **Nextcloud** – Provides the web-based cloud storage interface.
- **MariaDB** – Stores and manages the application's database information.

Docker Compose manages the communication between these services and allows them to run together as a single environment.

## Skills Gained

- Writing Docker Compose YAML files.
- Deploying multiple containers as one application.
- Configuring database connections.
- Using Docker commands for deployment and management.
- Working with port mapping for web applications.
- Applying Infrastructure as Code concepts.
- Documenting cloud deployment activities using Markdown.
