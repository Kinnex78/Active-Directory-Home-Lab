After setting the Adapters, i continued with installing the Windows-Server-2019. Because I wanted a user-friendly graphical interface, I chose the “Desktop Experience” option. It also reflects a more realistic real-world enterprise environment.

![Win-Server-2019 installation](screenshots/05-dc01-setup-installation.png)


After the installation was completed, I navigated to Settings → Network & Internet → Change adapter options.
I then renamed the network adapters from “Ethernet 1” and “Ethernet 2” to “EXTERNAL” and “INTERNAL” to clearly distinguish between the two network roles.

The EXTERNAL adapter was left on automatic configuration (DHCP), allowing it to obtain a dynamic IP address from the NAT network.
The INTERNAL adapter was configured with a static IP address to provide stable addressing for the domain environment.

![Win-Server-2019 Configure static IP for DNS-Connection](screenshots/06-dc01-configure-static-ip.png)
