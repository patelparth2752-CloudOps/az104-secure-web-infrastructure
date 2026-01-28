# Secure Web Infrastructure on Azure (AZ-104 Project)

This project demonstrates core Azure Administrator (AZ-104) skills by building a secure and monitored web infrastructure using Microsoft Azure.

The goal of this project is to showcase hands-on experience with Azure networking, security, compute, monitoring, and access control.

---

## Architecture Overview

The project includes:
- Azure Resource Group for organization
- Virtual Network with subnet
- Network Security Group (NSG) for traffic control
- Linux Virtual Machine hosting a web server
- Azure Monitor for performance monitoring
- Azure Backup for data protection
- Role-Based Access Control (RBAC)

---

## Azure Services Used

- Azure Resource Groups
- Azure Virtual Network (VNet)
- Subnets
- Network Security Groups (NSG)
- Azure Virtual Machine (Linux)
- Azure Monitor & Log Analytics
- Azure Backup
- Azure RBAC

---

## Security Implementation

- NSG allows HTTP (port 80) from the internet
- SSH (port 22) restricted to my public IP only
- Default deny rules enforced
- RBAC applied using least-privilege principle

---

## Monitoring and Backup

- VM Insights enabled using Azure Monitor
- Log Analytics workspace configured
- Backup enabled using Recovery Services Vault with daily backups

---

## Challenges Faced

- Encountered vCPU quota limits on a new Azure subscription
- Resolved by requesting a regional vCPU quota increase

---

## Future Improvements

- Add Load Balancer for high availability
- Automate deployment using ARM or Bicep
- Extend project with DevOps practices

---

## Author

Parth  
Azure Administrator (AZ-104 Certified)
