# architecture

This lab simulates a small enterprise Active Directory environment using VirtualBox.

                 +----------+
                 | Internet |
                 +----------+     
                       │
                       │
                Home Router/ISP
                       │
                       │
                    Host OS
               (VirtualBox Host)
                       │
                 VirtualBox NAT
                       │
                       │
        +--------------------------------+
        | DC01 – Windows Server 2019     |
        | Roles Installed:               |
        | - Active Directory Domain      |
        |   Services (AD DS)             |
        | - DNS Server                   |
        | - DHCP Server                  |
        | - RRAS (NAT Routing)           |
        |                                |
        | NIC1: EXTERNAL (NAT)           |
        | NIC2: INTERNAL (ADLAB)         |
        | IP: 172.16.0.10                |
        +--------------------------------+
                       │
                       │
            Internal Network (ADLAB)
               Subnet: 172.16.0.0/24
                       │
                       │
        +--------------------------------+
        | CLIENT1 – Windows 10 Pro       |
        | Domain Joined                  |
        | DHCP Client                    |
        | NIC1: ADLAB                    |
        +--------------------------------+

        
