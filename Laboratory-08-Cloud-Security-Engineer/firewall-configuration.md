# Firewall Configuration

## 1. Setting Up SSH Access

I allowed SSH connections so I can access the server remotely when needed.

```bash
sudo ufw allow 22/tcp
```

## 2. Setting the Firewall Policies

I configured UFW to reject incoming connections by default while allowing outgoing traffic. After setting the policies, I activated the firewall and checked its status.

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
```

## 3. Opening the Web Application Port

Since the Nginx web application uses port 8080, I added a firewall rule to allow TCP connections through that port.

```bash
sudo ufw allow 8080/tcp
sudo ufw status numbered
```

## 4. Importance of Allowing SSH

Allowing SSH before enabling the firewall helps prevent losing remote access to the server. If SSH is blocked, I may not be able to connect remotely. Firewall rules should be configured carefully to keep the server accessible while limiting unnecessary connections.

## Conclusion

Configuring UFW helped me understand how firewall rules control network traffic. By allowing only the required ports and blocking incoming connections by default, I can improve the security of the server.
