# Checkpoint 6 – Technical Documentation

## Mission Overview

The mission of this laboratory activity is to understand the basic concepts of cloud computing and how cloud infrastructure components work together. The activity focuses on identifying cloud resources, designing a simple cloud infrastructure, and documenting the tools and commands used during the laboratory exercises.

## Objectives

- Understand the basic concepts of cloud computing.
- Identify the major cloud providers such as AWS, Microsoft Azure, and Google Cloud Platform.
- Compare equivalent cloud infrastructure services.
- Design a simple cloud infrastructure for a fictional company.
- Understand the purpose of compute, storage, networking, and internet resources.
- Practice basic Linux commands used in cloud computing environments.
- Document the tools, skills, and challenges encountered during the laboratory activities.

## Cloud Infrastructure Components

The following are the main components used in the simple cloud infrastructure:

| Component | Description |
|---|---|
| **Compute Resource** | A virtual machine that provides processing power for applications and services. Examples include Amazon EC2, Azure Virtual Machines, and Google Compute Engine. |
| **Storage Resource** | A cloud storage service used to store files, images, backups, and other data. Examples include Amazon S3, Azure Blob Storage, and Google Cloud Storage. |
| **Network** | A virtual network that connects and manages communication between cloud resources. Examples include Amazon VPC, Azure VNet, and Google VPC. |
| **User** | The person who accesses the cloud application or services through a web browser or mobile application. |
| **Internet Connection** | Provides connectivity between the user and the cloud infrastructure through the internet. |

### Simple Cloud Architecture

```text
                  +----------------------+
                  |   Compute Resource   |
                  |   Virtual Machine    |
                  +----------+-----------+
                             |
                             |
+-------------+        +-----v-----+        +----------------------+
|    User     | <----> | Internet  | <----> | Storage Resource     |
| Web/Mobile  |        |           |        | Object Storage       |
+-------------+        +-----+-----+        +----------------------+
                             |
                       +-----v-----+
                       |  Network  |
                       |    VPC    |
                       +-----------+
                             |
                       +-----v-----+
                       | Internet  |
                       | Connection|
                       +-----------+
