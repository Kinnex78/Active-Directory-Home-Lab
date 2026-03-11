As described earlier, I enabled the DHCP option.
![Checking DHCP](screenshots/20-dhcp-on.png)

At this stage, I installed the DHCP Server role so that the client would automatically obtain an IP address in the next step.
![Installing DHCP](screenshots/21-install-dhcp.png)

After the installation, I authorized the DHCP server.
![Authorizing DHCP](screenshots/22-authorize-dhcp-in-ad.png)

Following the authorization, I navigated to Windows Administrative Tools → DHCP, then right-clicked on IPv4. 
![Open New Scope Wizard](screenshots/23-ipv4-new-scope.png)

When opening the New Scope Wizard, I first defined a scope name and description.
![Naming, describing Scope](screenshots/24-naming-scope.png)

Before configuring the DHCP scope, I verified the DNS server address and the subnet mask to ensure the correct network information.
![Checking DNS and Subnet mask first](screenshots/25-checking-dns-and-subnet-mask.png)

Afterwards, I defined the scope IP address range that should be assigned to clients and entered the subnet mask of the server network.
![Setting range, type in given Subnet mask](screenshots/26-destinate-dhcp-scope.png)

To allow the scope clients to use the correct DNS configuration, I entered the server name and the DNS server IP address. 
![Pairing Scope-Clients to DNS](screenshots/27-pairing-scope-clients-to-dns.png)

With these settings completed, the DHCP scope configuration was finalized.
![New Scope completed](screenshots/28-new-scope-completed.png)

