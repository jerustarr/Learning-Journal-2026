
## Promoting Windows Server → Domain Controller

### Set Static IP Address
- Open Settings → Network and Internet → Ethernet → IP Assignment
   - Under Edit IP Address
       - click manual and check **IPv4**
 - Assigning IP Address
     - IP Address
     - Subnet Mask
     - Preferred DNS = Server’s own IP
- Rename the Server (Optional)
    - If a rename is preferred, it must be done before promotion to avoid outages
- Reboot after renaming
- Using Server Manager
    - Open Server Manager
    - Click Add Roles and Features
    - Choose Role-based or feature-based installation
    - Select your current server
    - Check Active Directory Domain Services
    - Click Add Features when prompted
    - Click Next → Install
#### When installation has finished, you will see a yellow notification flag to promote the server  
## Promoting the Server to a Domain Controller 
- Click the yellow warning icon in server Manager
- Click promote this server to a domain controller
- Click Add a new forest
    - Set the name of your new domain
    - Example: lab.local
- Configure Domain Controller Options
- Set Forest Functional Level: Windows Server 2025
- Set Domain Functional Level: Windows Server 2025
- Set the DSRM Password
- Reboot the machine 
