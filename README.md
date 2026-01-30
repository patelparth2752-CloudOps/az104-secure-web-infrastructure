# Secure Web Infrastructure on Azure (AZ-104 Project)

## Overview
This project demonstrates the implementation of a secure and monitored web infrastructure on Microsoft Azure.  
It is designed as a hands-on AZ-104 level project to showcase core Azure Administrator skills.

## Architecture
- Resource Group
- Virtual Network with Subnet
- Network Security Group (NSG)
- Linux Virtual Machine (Ubuntu)
- Public IP
- Azure Monitor
- Azure Backup
- Role-Based Access Control (RBAC)
  
## Architecture Diagram (Daigram.png)
User (Browser)
     |
     | HTTP (Port 80)
     v
Public IP Address
     |
     v
Network Security Group (NSG)
     |
     v
Virtual Network (VNet)
     |
     v
Subnet
     |
     v
Linux VM (Ubuntu)
     |
     v
Nginx Web Server

![Architecture Overview](screenshots/daigram.png)
    
## Azure Services Used
- Azure Virtual Machines
- Azure Virtual Network
- Network Security Groups
- Azure Monitor
- Azure Backup
- Microsoft Entra ID (RBAC)

## Implementation Steps
1. Created a Resource Group for isolation and management
2. Configured a Virtual Network and Subnet
3. Created and associated NSG with inbound rules (HTTP, SSH)
4. Deployed a Linux VM inside the VNet
5. Installed and configured Nginx web server
6. Verified web access using Public IP
7. Enabled Azure Monitor and collected metrics
8. Configured Azure Backup for the VM
9. Applied RBAC with least-privilege access

## Validation & Evidence
Screenshots are included to validate:
- VM deployment
- Nginx web page access
- NSG rules
- Monitoring metrics
- Backup configuration
- RBAC assignment

## Security Considerations
- Restricted inbound traffic using NSG
- SSH access limited
- Role-based access control applied
- Backup enabled for disaster recovery

## Outcome
This project demonstrates practical experience with Azure core infrastructure, security, monitoring, and governance aligned with AZ-104 objectives.
