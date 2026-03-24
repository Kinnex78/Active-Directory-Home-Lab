Next, I opened the Server Manager Dashboard and selected “Add Roles and Features.”
Under Server Roles, I chose Active Directory Domain Services (AD DS).

![Installing ADDS](screenshots/07-adds-install.png)


I also selected Domain Name System (DNS) Server to ensure proper name resolution within the domain environment.

![Installing DNS](screenshots/08-dns-install.png)


After the required roles were installed, I proceeded to promote the server to a Domain Controller using the post-deployment configuration wizard.

![Promote to DC](screenshots/09-promote-to-dc.png)


During the domain controller promotion process, I configured the server to create a new forest.

![Adding a new forest](screenshots/10-add-new-forest.png)


I then defined the Directory Services Restore Mode (DSRM) password, which is required for recovery and maintenance operations.

![Setting DRSM-password](screenshots/11-setting-drsm-pw.png)


The automatically generated NetBIOS domain name was reviewed and kept unchanged.

![Kept Net-BIOS](screenshots/12-keep-NetBIOS.png)


After confirming the configuration settings, the installation process began. Upon completion, the system performed an automatic restart to finalize the domain controller setup.
