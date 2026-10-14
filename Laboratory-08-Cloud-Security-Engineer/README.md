# Laboratory 08: Cloud Security Engineer

## Mission Overview

In this laboratory, I learned how to improve server security by setting up a firewall using UFW. I configured the firewall to block unwanted incoming connections while allowing outgoing traffic and necessary services.

## Objectives

- Learn the importance of server security.
- Understand how a firewall protects a server.
- Set default rules for incoming and outgoing traffic.
- Allow required ports for SSH and web applications.
- Check firewall settings to confirm the configuration.

## Commands Used

```bash
docker run -d -p 8080:80 --name secure-web-app nginx
curl http://localhost:8080
sudo ufw allow 22/tcp
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
sudo ufw allow 8080/tcp
sudo ufw status numbered
```

## Skills Learned

- Deploying an Nginx container using Docker.
- Testing a web application through a local port.
- Setting up firewall rules with UFW.
- Blocking unwanted incoming connections.
- Verifying and managing allowed network ports.

## Conclusion

This activity helped me understand how to protect a server by controlling network connections. I also learned that checking firewall rules is important to ensure that only the necessary services are accessible.
