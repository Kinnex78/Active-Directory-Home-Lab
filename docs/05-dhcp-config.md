As described earlier on i've now checked the DHCP-box.
![Checking DHCP](screenshots/20-dhcp-on.png)

And here i installed DHCP Server, so that the Client gets an IP automatically at the next step.
![Installing DHCP](screenshots/21-install-dhcp.png)

Then, i just authorized DHCP up here.
![Authorizing DHCP](screenshots/22-authorize-dhcp-in-ad.png)

Following to the authorization, i navigated to "Windows Administrative Tools" -> double-click on "DHCP" -> right-click on "IPv4" 
![Open New Scope Wizard](screenshots/23-ipv4-new-scope.png)

By opening the Wizard, i first gave the scope following name, same as description.
![Naming, describing Scope](screenshots/24-naming-scope.png)

Before destinating the DHCP-Scope, i looked up my DNS, same as the Subnet-mask, to type in these informations corecctly.
![Checking DNS and Subnet mask first](screenshots/25-checking-dns-and-subnet-mask.png)

Afterwards, i set the range of Scope, which IP-addresses i inlcude for now, and typed in the number of my Servers Subnet mask.
![Setting range, type in given Subnet mask](screenshots/26-destinate-dhcp-scope.png)

To pair Scope-Clients with my DNS i also typed in my Server-name, same as my IP-address. 
![Pairing Scope-Clients to DNS](screenshots/27-pairing-scope-clients-to-dns.png)

And now, the DHCP-Scope-Configuration is completed
![New Scope completed](screenshots/28-new-scope-completed.png)

