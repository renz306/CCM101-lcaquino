# System Baseline Report

## Server Resource Check

Before running the client website, I checked the server's resources to know its current condition and available capacity.

### 1. Memory Usage

I used the `free -h` command to check the total memory, used memory, and available RAM. This helps me understand if the server has enough memory to run its applications.

**Command:**

```bash
free -h
```

### 2. Disk Space

I checked the available storage of the root directory using the `df -h /` command. This helps me determine how much disk space is still available.

**Command:**

```bash
df -h /
```

### 3. CPU and Running Processes

I used the `top` command to monitor CPU activity and see which processes are currently running. This is useful for identifying processes that consume too many system resources.

**Command:**

```bash
top
```

## Importance of System Monitoring

Checking system resources before deploying an application helps prevent performance issues. Enough disk space is needed to store logs, files, and temporary data. Regular monitoring also helps identify resource problems early and keeps the server running properly.

