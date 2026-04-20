# Day 5 - Networking and Ports

## 📌 Objective
Learn AWS networking concepts including VPC Peering, NAT Gateway, routing, and port connectivity testing.

---

## ✅ Tasks Completed

- Created 2 VPCs  
- Established VPC Peering connection  
- Launched EC2 instances in both VPCs  
- Configured route tables for peering communication  
- Verified private connectivity between instances  

- Created a VPC for NAT setup  
- Created public and private subnets  
- Attached Internet Gateway to public subnet  
- Created NAT Gateway in public subnet  
- Configured route tables for NAT routing  
- Launched EC2 instances in public and private subnets  

 

---

## 🛠️ Commands Used

```bash
# Connectivity
ping <private-ip>
ssh <instance-ip>


# Testing
curl http://<public-ip>
telnet <ip> 80
