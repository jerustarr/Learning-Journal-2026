## Navigating Active Directory Users and Computers 

### Overview 
tbw 
## Creating Organisational Units (OU)

#### Create the Organizational Units (OUs) that will store the different user and computer objects used in the tiered access model.

**General Steps:** 
1.	Open Active Directory Users and Computers.
2.	Right click the domain → New → Organizational Unit.
3.	Create the required OUs for your environment, e.g.:
   -  User OUs (Tier 0 / Tier 1 / Tier 2 users)
   -  Computer OUs (Tier 1 servers / Tier 2 workstations)
4.	Move the appropriate user and computer accounts into their respective OUs.

## Creating Security Groups  
#### Create security groups that will control which tier the user belongs to.
**General Steps:**
1.	In ADUC, navigate to the OU where you store groups.
2.	Right click → New → Group.
3.	Create the necessary groups, such as (examples only):
   - Tier0-Admin-Access (optional; Domain Admins can also act as Tier 0)
   - Tier1-Server-Access
   - Tier2-User 
4.	Ensure all groups are created as Security → Global groups.

### Creating User
Create one user for each tier and place them in the correct OU.
**General Steps:**
1.	Navigate to the target OU (e.g., Tier1-Admins or Tier2-Users).
2.	Right click → New → User.
3.	Enter user details (name, username, password).
4.	Complete the wizard to create the account.

## Add User to Security Groups 
Assign each user to the correct tier-based security group so the script can identify their level of access.
**General Steps:**
1.	Open the user account.
2.	Go to the Member Of Tab.
3.	Click Add…
4.	Add the user to the group that matches their tier:
      - Tier 0 user → Domain Admins (and/or Tier0-Admin-Access)
      - Tier 1 user → Tier1-Server-Access
      - Tier 2 user → Tier2-User
5.	Apply and close.

