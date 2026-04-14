# Day 1 - Ubuntu Setup using AWS EC2

## Objective
Install Ubuntu server 3 times:
- 2 manual setups
- 1 automated setup using user-data (cloud-init)

---

## What I Did

### Instance 1 (Manual Setup)
- Launched Ubuntu EC2 instance
- Connected using EC2 Instance Connect
- Installed nginx manually using:
  sudo apt-get update -y
  sudo apt-get install nginx -y

---

### Instance 2 (Manual Setup)
- Repeated the same process
- Practiced server setup again

---

### Instance 3 (Automated Setup)

Used user-data script to automate installation:

```bash
#!/bin/bash
sleep 60
apt-get update -y
apt-get install -y nginx
systemctl start nginx
systemctl enable nginx
echo "Hello from Automated Server" > /var/www/html/index.html






