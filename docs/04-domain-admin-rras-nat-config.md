Via Tools → Active Directory Users and Computers, I right-clicked on lab.local, selected New → Organizational Unit, and created an OU named “AdminAccounts.”

Inside this OU, I selected Create a new user in the current container and defined the First name, Last name, Full name, and User logon name.

After setting the designated password, I unchecked “User must change password at next logon” and checked “Password never expires.”
![Creating Domain Admin](screenshots/14-create-domain-admin.png)

Lastly, I opened the created user account, navigated to the Member Of tab, clicked Add…, and entered “Domain Admins” in the Object names to select field to assign the user to the Domain Admin group.
![Giving Admin-privilege](screenshots/15-giving-admin-privilege.png)

After creating the Domain Admin account, I proceeded with installing RRAS by navigating to Add Roles and Features and selecting the role Remote Access.
![Checking box RAS](screenshots/16-choosing-ras.png)

Under Role Services, I selected Routing, which automatically also enabled DirectAccess and VPN (RAS).
![Checking box Routing](screenshots/17-choosing-routing.png)

After this, i continued to install those features.

After the installation was completed, I navigated to Tools → Routing and Remote Access, right-clicked the designated server, selected Configure and Enable Routing and Remote Access, chose Network Address Translation (NAT),
![Choose NAT](screenshots/18-choosing-nat.png)

and configured the EXTERNAL interface as the public interface using “Use this public interface."
![Choose public interface: EXTERNAL](screenshots/19-choosing-public-interface-external.png)
