# Cloud Infrastructure Components

## Checkpoint 3 – Identify Cloud Infrastructure Components

Based on the investigation of the Linux cloud server in KillerCoda, the following cloud infrastructure components were identified.

---

## 1. Compute Resources

### Example
- **CPU:** Intel Xeon E312xx (Sandy Bridge, IBRS update)
- **CPU Cores:** 1
- **CPU Threads:** 1
- **CPU Speed:** 2.0GHz
- **Virtualization:** KVM

### Purpose
Compute resources provide the processing power needed to run applications, execute commands, and perform tasks on the cloud server.

### Importance in Cloud Computing
Compute resources are important because cloud applications need CPU power to process data, run services, and handle user requests. Cloud providers can allocate different amounts of CPU resources depending on the needs of the workload.

### Relation to the KillerCoda Linux Environment
The KillerCoda environment provides a virtual cloud server with an Intel Xeon CPU and 1 CPU core. The server runs through KVM virtualization, allowing the Linux environment to operate as a virtual machine.

---

## 2. Storage Resources

### Example
- **Main Disk:** 19 GiB
- **Used Storage:** 5.4 GiB
- **Available Storage:** 13 GiB
- **Boot Partition:** 881 MiB
- **EFI Partition:** 105 MiB

### Purpose
Storage resources are used to store the operating system, applications, configuration files, user files, and other data required by the server.

### Importance in Cloud Computing
Storage is important because cloud servers need persistent space for operating system files, applications, databases, logs, and other information. Adequate storage allows applications and services to operate properly.

### Relation to the KillerCoda Linux Environment
The KillerCoda server has a 19 GiB main disk mounted at `/`. It also has separate `/boot` and `/boot/efi` partitions. The `df -h` command was used to inspect the available storage and mounted file systems.

---

## 3. Networking Resources

### Example
- **Hostname:** ubuntu
- **Primary IP Address:** 172.30.1.2
- **Network Interface:** enp1s0
- **Docker IP Address:** 172.17.0.1
- **Loopback Address:** 127.0.0.1

### Purpose
Networking resources allow the cloud server to communicate with other systems, services, and networks.

### Importance in Cloud Computing
Networking is important because cloud servers need network connectivity to communicate with users, applications, databases, and other cloud resources. IP addresses and network interfaces allow data to be transmitted between systems.

### Relation to the KillerCoda Linux Environment
The KillerCoda Linux server uses the `enp1s0` network interface with the primary IP address `172.30.1.2`. It also has a Docker network interface using `172.17.0.1`. These network resources allow the virtual server and its services to communicate within their respective networks.

---

## 4. Operating System

### Example
- **Operating System:** Ubuntu 24.04.4 LTS
- **Codename:** Noble Numbat
- **Kernel:** 6.8.0-138-generic
- **Architecture:** x86_64

### Purpose
The operating system manages the server's hardware and software resources. It provides the environment needed to run applications, execute commands, manage files, and configure networking.

### Importance in Cloud Computing
The operating system is important because cloud applications and services need an operating environment to run. It manages CPU, memory, storage, networking, users, processes, and other system resources.

### Relation to the KillerCoda Linux Environment
The KillerCoda cloud server runs Ubuntu 24.04.4 LTS with the 6.8.0-138-generic Linux kernel. The x86_64 architecture allows the system to run 64-bit Linux applications and services.

---

## Summary

| Cloud Component | KillerCoda Example | Purpose |
|---|---|---|
| Compute Resources | Intel Xeon E312xx, 1 CPU Core | Provides processing power |
| Storage Resources | 19 GiB Main Disk | Stores the OS, applications, and data |
| Networking Resources | 172.30.1.2, enp1s0 | Provides network communication |
| Operating System | Ubuntu 24.04.4 LTS | Manages hardware and software resources |

---

## Conclusion

The investigation of the KillerCoda Linux environment demonstrates the main components of cloud infrastructure. The server uses compute resources through an Intel Xeon processor, storage resources through a 19 GiB disk, networking resources through its network interfaces and IP addresses, and Ubuntu 24.04.4 LTS as its operating system. These components work together to provide a functional cloud computing environment where applications and services can run.
