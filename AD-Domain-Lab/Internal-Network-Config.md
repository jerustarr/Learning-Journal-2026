## Internal Network Set-Up

### Background Information 
To successfully join a workstation to the domain, both the Domain Controller and the client must reside on the same internal network. The Default Switch used during initial setup provides internet connectivity but does not allow direct communication between VMs. By configuring all VMs to use the same internal virtual switch, we ensure they share a common subnet and can resolve each other’s names. Since the Domain Controller provides DNS and authentication services, the workstation’s DNS must point to the Domain Controller’s IP address. This setup guarantees proper name resolution and connectivity, which are prerequisites for joining the domain.

#### To start...  
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
