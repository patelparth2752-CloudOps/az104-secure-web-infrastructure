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
  
## Architecture Overview
The solution follows a standard Azure single-VM web architecture designed with security and network isolation in mind. End users access the application through a web browser over HTTP on port 80 via an Azure Public IP address.

Inbound traffic is controlled using a Network Security Group (NSG), which enforces access rules and allows only required ports before traffic enters the virtual network. The workload is deployed inside a Virtual Network (VNet) and routed to a dedicated subnet to ensure logical separation and isolation.

A Linux virtual machine running Ubuntu is deployed within the subnet and hosts an Nginx web server to serve HTTP requests. This architecture demonstrates practical implementation of Azure networking, security controls, and compute services aligned with Azure Administrator (AZ-104) responsibilities.

![Architecture Overview](screenshots/v-net.png)
    
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


## Security Considerations
- Restricted inbound traffic using NSG
- SSH access limited
- Role-based access control applied
- Backup enabled for disaster recovery

## Outcome
This project demonstrates practical experience with Azure core infrastructure, security, monitoring, and governance aligned with AZ-104 objectives.
