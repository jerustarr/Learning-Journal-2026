## Creating Active Directory Domain Controller (AD/DC)

### Background Knowledge 
Active Directory (AD) is a directory service developed by Microsoft for Windows domain networks. Active Directory is essentially a database that holds all the relevant information about users and endpoint. This includes servers and storage. AD also provides a suite of directory services that associate those network resources with their network addresses, ensuring that information is available to the entire network. In addition, AD handles security, such as authentication to ensure that only valid users are allowed onto the network, and authorization to ensure that valid users can access only resources to which they're entitled.

A domain controller is a server that runs on the the Active Directory Domain Services (AD DS) role. It authenticates and authorizes all users and computers in a Windows domain-type network. It assigns and enforces security policies for all computers including installing and updating softwares!

Think of it as a school or work domain joined computer along with the privileges each user account has! 

### Learning Purposes 
- Setting up windows 11 
-  Setting up Windows Server 2025
      - Promoting Windows Server to DC
-  A Brief introduction to internal networking
      - Testing network connectivity
- Joining the domain
- Tier structure and principle of least privilege 
- Basic usage of AD/DC 

### Prerequisties
Windows or any machine using **x64** is required for this home lab. Windows Server ISO for **arm64** is not available hence this setup cannot be recreated on any machines using M1/2/3 chips.
Prior knowledge on the usage and navigation of hypervisors and virtual machines (guide on setting up environment --> AD-Domain-Lab/VM-Setup)

### To start
Start from **VM-Setup** --> **Server-Setup**

#### References 
https://www.techtarget.com/searchwindowsserver/definition/Active-Directory-domain-AD-domain
