# AWS EC2 + IAM + S3 Hands-On Lab

## Project Overview
This project demonstrates practical implementation of AWS core services including EC2, IAM, and S3. The goal is to understand secure access management, instance configuration, and service integration using IAM Roles.

---

## Key Concepts Covered
- EC2 instance setup and configuration  
- Security Groups (firewall rules)  
- IAM Users vs IAM Roles  
- Policy-based access control  
- Secure access to S3 without access keys  

---

##  Architecture
User → IAM → EC2 Instance → IAM Role → S3 Bucket

---

##  Steps Performed

### 1. Launch EC2 Instance
- Created an EC2 instance (Amazon Linux)
- Configured Security Group:
  - SSH (Port 22) → My IP
  - HTTP (Port 80) → Anywhere

---

### 2. Install Web Server
```bash
sudo yum install httpd -y
sudo systemctl start httpd
