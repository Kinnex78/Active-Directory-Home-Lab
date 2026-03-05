Via "Tools"->"Active Directory Users and Computers"->rightclick on "lab.local" and choosing "New"->Organisational Unit,
i've created an UO called "AdminAccounts". Then by clicking on this UO and selecting "create a current User in the current container" I've set the "User logon name" also like the First- Last- and Full name.
Following with choosing the destinated password i've also unchecked "User must change password at next logon" and checked the box "password never expires".
![Creating Domain Admin](screenshots/14-create-domain-admin.png)

Lastly, by rightclicking (or doubleclicking) on destinated User i navigated to "Member of" and clicked on "Add..." to type in "Domain Admin" in the large Textfield, the "object name to select"-field.
![Giving Admin-privilege](screenshots/15-giving-admin-privilege.png)

After creating the Domain-Admin i proceeded with installing RRAS by navigating to "Add roles and features" and checking the box "Remote Access".
![Checking box RAS](screenshots/16-choosing-ras.png)

Also the same at "Role Services" by choosing "Routing" which also automatically checking the box "DirectAccess and VPN (RAS)"
![Checking box Routing](screenshots/17-choosing-routing.png)

After this, i continued to install those features.
