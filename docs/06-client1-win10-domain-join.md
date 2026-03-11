I started by Installing the Client.
![Installation](screenshots/29.2-restarting-installation.png)

When i prepared the join, i've first checked if DHCP is received on the Client. On the Screenshot you can see that DHCP is enabled.
(But you can also see the first Error, which represents that the DNS isnt recognized properly.)
![DHCP enabled](screenshots/29-checking-dhcp-recievement.png)

After fixing the DNS-Problem u can read in 08-troubleshooting, i then started loging in with my Domain-Admin i created earlier on, and also typed in the password as well as the Domain name.
![Domain-Join1](screenshots/30-domain-join-type-domain-infos.png)

Then, i typed in the Domain Controller and the Computer Domain again.
![Domain-Join2](screenshots/31-typing-in-domain-infos.png)

and finally logged in with the User's credentials (Domain Admin), but instad of "LAB/Wolffried-admin" i typed in wolffried-admin@lab.local.
![Domain-Log-on](screenshots/32-logging-in-domain.png)

So now it forces a restart.
![Domain-Log-on-succeed](screenshots/33-joind-succeed-restart-now.png)

While forcing a restart, the vm stucked while loading. So i decided to force the restart via "ctrl + R". The Process of joining the domain didnt vanished, so i normally logged in.
![Logging in after restart](screenshots/34-restart-stucked-forced-a-vm-restart-logging-in.png)

and thats it for now.
