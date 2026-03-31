# Active-Directory-Home-Lab
## Overview

This project documents the design and implementation of a small Active Directory lab environment using Windows Server 2019 and Windows 10 Pro within Oracle VirtualBox.

The lab simulates a basic enterprise network infrastructure and was created to deepen my understanding of system administration, network services, and virtualization.

To ensure safe experimentation while maintaining internet access, the environment is isolated using a combination of **NAT** and **Internal Network** configurations.

---

## Lab Environment

### Domain Controller

- **Hostname:** DC01  
- **Operating System:** Windows Server 2019  
- **Roles:**
  - Active Directory Domain Services (AD DS)
  - DNS Server
  - DHCP Server
  - Routing and Remote Access (RRAS)

### Client Machine

- **Hostname:** CLIENT1  
- **Operating System:** Windows 10 Pro  
- **Configuration:**
  - Domain joined (`lab.local`)
  - Receives IP configuration via DHCP

---

## Network Design

- **Internal Network:** `ADLAB`  
- **Subnet:** `172.16.0.0/24`  

| Component | IP Address |
|----------|-----------|
| DC01 | 172.16.0.10 |
| DHCP Range | 172.16.0.100 – 172.16.0.200 |
| Gateway | 172.16.0.10 |
| DNS Server | 172.16.0.10 |

The domain controller acts as:
- DNS server for name resolution  
- DHCP server for IP assignment  
- NAT router (via RRAS) for internet access  

---

## Learning Objectives

- Document the setup of an IT infrastructure project  
- Understand the core concepts of Active Directory and domain environments  
- Gain hands-on experience with virtualization using VirtualBox  
- Configure and manage a Domain Controller in a controlled environment  
- Implement and understand essential network services (DNS, DHCP, NAT)  
- Develop troubleshooting and problem-solving skills during deployment  

---

## Repository Structure

docs/       → Step-by-step setup documentation  
config/     → IP plan and infrastructure notes  
diagrams/   → Network topology diagrams  

## Validation

The lab environment was successfully validated with the following checks:

- Client receives IP configuration via DHCP  
- Client successfully joins the domain  
- DNS resolution is functional  
- Domain authentication works  
- Client has internet access through RRAS NAT

## References

### Documentation

- Microsoft Learn – Windows Server Documentation  
  https://learn.microsoft.com/windows-server/

- Oracle VirtualBox Networking  
  https://www.virtualbox.org/manual/ch06.html  

### GitHub Repositories (Inspiration & Reference)

- Active Directory Lab (aashraymt)  
  https://github.com/aashraymt/AD-Lab  
