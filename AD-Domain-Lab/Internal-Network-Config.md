## Internal Network Set-Up

### Background Information 


#### To start... 
To join the domain, we have to ensure that both the server and the workstations are on the same internal network. Initially during setup, we had the VM's network adapter settings set to Default Switch tp ensure a smooth download of all required files. However, to ensure that the VMs can communicate with each other, we have to ensure to ensure that the network adapter settings is the exact same as the VMs we are trying to connect with. 
- Navigate to the current VM’s settings → Network Adapter
- Set Network Adapter to the exact same internal switch used by the Domain Controller
### Network Configuration 
- Open Settings → Network and Internet → Ethernet → IP Assignment
- Check Manual
- Assign
    - IP Address
    - Subnet Mask
    - Preferred DNS = Domain Controller’s IP
- Navigate to terminal

### Checking Basic Network connectivity
- Ping Domain Controller’s IP to check for basic network connectivity test and to ensure DNS can resolve itself
    - Ping ip address
    - Ping Hostname
    - Ping Fullt Qualified Domain Name (FQDN)
 
### JOINING THE DOMAIN 
#### Ensure ping connectivity works 
- Navigate to settings → Accounts → Add a work or school account
- Click connect
- Click Join this device to a local Active Directory Domain
- Enter domain name when prompted
- Enter domain controller’s admin account when prompted 
