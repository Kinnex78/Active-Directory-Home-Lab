
First, I navigated to File → Tools → Network Manager and opened the NAT Network tab to configure the external network. I then created a network named “NAT-LAB”, assigned an IPv4 prefix, and disabled DHCP in order to configure the addressing manually later via Server Manager.

![VBox NAT-Network setup](screenshots/05-vbox-tools-network-config.png)


After completing the Server Setup Wizard, I configured the network adapters. The first adapter was assigned to the External Network.

![Server Adapter 1](screenshots/01-vbox-adapter-extern-server.png)


The second adapter was configured as the Internal Network.

![Server Adapter 2](screenshots/02-vbox-adapter-intern-server.png)


The same configuration was applied to the Windows 10 Pro client, where the first adapter was connected to the External Network.

![Client Adapter 1](screenshots/03-vbox-adapter-extern-client.png)


The second adapter of the client was configured as the Internal Network.

![Client Adapter 2](screenshots/04-vbox-adapter-intern-client.png)
