# Cloud Infrastructure Report

## Investigation Date
August 30, 2026

## Investigator
Laurenz Christian A. Aquino

---

## Server Specifications

### 1. Operating System

- **\*Distribution\***: Ubuntu 24.04.4 LTS
- **\*Codename\***: Noble Numbat
- **\*Kernel Version\***: 6.8.0-138-generic
- **\*Architecture\***: x86_64

---

### 2. Kernel Information

- **\*Version\***: 6.8.0-138-generic
- **\*Build Date\***: Fri Jul 31 22:41:49 UTC 2026
- **\*Kernel Type\***: PREEMPT_DYNAMIC

---

### 3. CPU Specifications

- **\*Model\***: Intel Xeon E312xx (Sandy Bridge, IBRS update)
- **\*CPU Speed\***: 2.0GHz
- **\*CPU Cores\***: 1
- **\*Threads\***: 1
- **\*Sockets\***: 1
- **\*Cache\***: L1=32KB, L2=4MB, L3=16MB
- **\*Hypervisor\***: KVM

---

### 4. Memory (RAM)

- **\*Total RAM\***: 1.9 GiB
- **\*Used RAM\***: 423 MiB
- **\*Free RAM\***: 832 MiB
- **\*Available RAM\***: 1.4 GiB
- **\*Swap\***: 1.0 GiB

---

### 5. Storage (Disk)

- **\*Main Disk\***: 19 GiB (5.4 GiB used, 13 GiB available)
- **\*Boot Partition\***: 881 MiB (117 MiB used, 703 MiB available)
- **\*EFI Partition\***: 105 MiB (6.2 MiB used, 99 MiB available)

---

### 6. Mounted File Systems

- **\*/\***: /dev/vda1
- **\*/boot\***: /dev/vda16
- **\*/boot/efi\***: /dev/vda15
- **\*/run\***: tmpfs
- **\*/dev/shm\***: tmpfs
- **\*/run/lock\***: tmpfs

---

### 7. Network Configuration

- **\*Hostname\***: ubuntu
- **\*Primary IP\***: 172.30.1.2
- **\*Secondary IP\***: 172.17.0.1 (Docker)
- **\*Network Interface\***: enp1s0
- **\*Loopback IP\***: 127.0.0.1

---

## Investigation Commands

The following commands were used to investigate the cloud server:

```bash
uname -a
uname -r
cat /etc/os-release
lscpu
free -h
df -h
ip a
hostname -I
