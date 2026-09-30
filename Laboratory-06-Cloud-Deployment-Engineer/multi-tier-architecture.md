# Multi-Tier Architecture – Nextcloud Deployment

A multi-tier architecture divides an application into separate layers, where each layer has a specific responsibility. In this deployment, Nextcloud and MariaDB are organized into two main tiers.

## Application Tier

The application tier is handled by the **Nextcloud container**. It provides the web interface where users access the cloud storage system. It also processes requests, manages uploaded files, and performs the application's main functions.

Users can access Nextcloud through the configured **port 8080**.

## Database Tier

The database tier is provided by the **MariaDB container**. It is responsible for storing information required by Nextcloud, including user data, account details, file information, and other application records.

The database communicates with Nextcloud internally and does not need to be directly accessible by users.

## Benefits of the Two-Tier Setup

Separating the application and database services makes the deployment easier to manage. Each service has a clear responsibility, while Docker Compose handles their connection.

This structure also improves organization and security because the database can remain inside the internal Docker network. It also makes it easier to maintain or modify individual services when needed.

## Architecture Flow

```text
User
  |
  v
Nextcloud Application
  |
  v
MariaDB Database
