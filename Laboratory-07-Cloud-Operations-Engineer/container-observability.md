# Container Observability Report

## 1. Checking Application Logs

To review the activities of my Nginx container, I executed this command:

```bash
docker logs client-website
```

The output displayed the requests received by the web server. It included successful page requests and an unsuccessful request to a page that does not exist.

### Error Log (HTTP 404)

```text
Copy the actual 404 log line from your terminal here.
```

Logs help administrators understand application activities and locate errors. They are useful for finding the cause of problems and checking how the application responds to user requests.

## 2. Monitoring Container Performance

I monitored the running container with the command:

```bash
docker stats
```

This command shows the current resource consumption of Docker containers.

Based on my observation, the container had the following measurements:

* **Container:** client-website
* **CPU Usage:** 0.00%
* **Memory Usage:** 2.73 MiB / 1.859 GiB
* **Memory Percentage:** 0.14%
* **Network I/O:** 3.77 kB / 5.29 kB

These measurements help determine whether the container is using too much CPU or memory while running.

## 3. Summary

Monitoring logs and resource metrics is important when managing a web server. Logs help identify requests and errors, while metrics show the resources used by the container. Combining these two methods helps administrators check application performance and troubleshoot problems more effectively.

