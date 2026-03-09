[1.During installation Windows-10-Pro-Client]

So during the installation of Windows 10 Pro i encountered the first error, which tells me that it isnt able too boot properly.
![Windows-10-Pro-Machine cant boot](screenshots/29.1-install-error.png)

First i've added one more core, because it might caused because it could lack of Processor-performance.
![Adding one more Core](screenshots/29.2-adding-one-core.png)

After trying again, the error still appears, so i powered off and startet the Win-Client. I immediatly pressed a key to restart the installation again.
![Renew Installation](screenshots/29.3-restarting-installation.png)

[2.On Client, DNS isnt given as it should be]

Next Error happend while trying to connect the Client with the Domain, lab.local. While an Error-Message appeared, as be seen in the followibg picture:
![Error: Domain couldn't be found](screenshots/29.4-error-domain-could-not-be-found.png)

As i proceed with checking if the DNS is matching, i saw by typing in: "ipconfig /all" 
that the output didnt give out the right IP, as actually no DNS was given at all.
![No matching DNS from output readable](screenshots/29.5-dns-isnt-wired.png)

I then powered on the DC, and checked if the right DNS frequently was shouted out, on the DHCP scope. I navigated to "Server Manager" -> "Tools" -> "DHCP" -> clicked on the Server and went through "IPv4" to "Scope" then to given-"Scope" and to "Scope options" as well as looked out for "006 DNS Servers". But the DNS seems right by now.
![Checking if right DNS is shouted via DHCP-Scope](screenshots/29.6-checked-out-006-dns-servers.png)

To be clear about the given DNS as it matches with the DC's IP, i headed over to the CMD and typed in: "ipconfig". And it also confirms the match between DC's IP with the DNS. So by now, it factors out the "DNS incompability".
![Checking if DC's IP is matching with DNS](screenshots/29.7-dns-matches-with-dc-ip.png)

As i parallel, tested "nslookup lab.local", it gave out the right dns, by now.
![nslookup lab.local on Client](screenshots/29.8-nslookup-lab.local-on-client.png)

So now, it may be able to connect due to powerring on the DC.
