# Laboratory 07: Cloud Operations Engineer

## Mission Overview

In this activity, I learned how to monitor a Linux server and manage a web application using Docker. I used Nginx to simulate a website, sent HTTP requests, checked application logs, and monitored the container's CPU and memory usage.

## Objectives

* Check the server's RAM and disk capacity.
* Run an Nginx container using Docker.
* Generate web requests and test an invalid page.
* View application logs and identify errors.
* Monitor container performance using `docker stats`.
* Document the results and screenshots in GitHub.

## Monitoring Commands Executed

| Command                      | Purpose                           |
| ---------------------------- | --------------------------------- |
| `free -h`                    | Check memory usage                |
| `df -h /`                    | Check disk capacity               |
| `top`                        | Monitor CPU and running processes |
| `docker ps`                  | View running containers           |
| `curl http://localhost:8080` | Test the website                  |
| `docker logs client-website` | View application logs             |
| `docker stats`               | Monitor CPU and memory usage      |

## Skills Learned

Through this laboratory activity, I practiced using Linux commands and Docker for basic server monitoring. I learned how to generate website traffic, check HTTP errors, read container logs, and observe resource consumption. These skills help me understand how to identify problems and maintain a running web application.

## Screenshots

The `screenshots` folder contains evidence of the server checks, Nginx deployment, HTTP requests, application logs, and container metrics.

