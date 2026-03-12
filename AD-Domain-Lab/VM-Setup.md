# A quick guide on setting up Virtual Machines! 

#### Note: This guide uses HyperV which is only available on Windows 10 and above Pro/Enterprise versions! If using Windows Home, other hypervisors like such as VirtualBox will be required. Set-up may vary slightly but the basic steps remain the same! 

### Before starting... 
Make sure you have downloaded a bootable ISO. 
An ISO contains the necessary files required to boot a computer to recover or reinstall an OS, using a CD, DVD, or a USB drive. This file consists a boot loader, an operating system, and other required files to allow the computer to boot directly into that environment. 

You can download ISOs directly from the microsoft webpage!

[Windows Server 2022 ISO](https://www.microsoft.com/en-us/evalcenter/download-windows-server-2022?msockid=31a5701fbf786db6327c66ebbe846c15)

[Windows 11 ISO](https://www.microsoft.com/en-us/software-download/windows11?msockid=31a5701fbf786db6327c66ebbe846c15)

## Creating a VM in HYPER-V 
- LAUNCH MICROSOFT HYPER-V
- Start Microsoft Hyper-V Manager
- Select New --> Virtual Machine

## Setting up Windows Server 2025
- Specify Name and Location
- Rename VM
- Uncheck the checkbox: Store the virtual machine in a different location
- Specify Generation
    - Select Generation 2
    - This provides support for newer virtualization features, UEFI-based firmware and supported 64-bit guest operating system
- Assign Memory
    - Assign at least 8 GB of memory
    - Check the checkbox: Use Dynamic memory for this virtual machine
- Configure Networking
    - Set connection to Internal Switch
- Connect Virtual Hard Disk
    - Create a new virtual hard disk
- Installation Options
    - Check the checkbox: Install an Operating System from a bootable CD/DVD-ROM
        - Check the checkbox: Image file (.iso)
        - Choose Browse to find and select the ISO file required for Windows Server
- Launch Windows Server VM
    -  Connect to the Windows Server VM
    -  Follow the steps to set language, keyboard options
    -  Select Install Server 2025 Datacenter – Desktop Experience
## Setting up Windows 11 
Specify Name and Location
- Rename VM
- Uncheck the checkbox: Store the virtual machine in a different location
- Specify Generation
    - Select Generation 2
    - This provides support for newer virtualization features, UEFI-based firmware and supported 64-bit guest operating system
- Assign Memory
    - Assign at least 8 GB of memory
    - Check the checkbox: Use Dynamic memory for this virtual machine
- Configure Networking
    - Set connection to External Switch
- Connect Virtual Hard Disk
    - Create a new virtual hard disk
- Installation Options
    - Check the checkbox: Install an Operating System from a bootable CD/DVD-ROM
        - Check the checkbox: Image file (.iso)
        - Choose Browse to find and select the ISO file required for Windows 11
-  Launch Windows Server VM
    -  Connect to the Windows 11 VM
    -  Follow the steps to set language, keyboard options
    -  Select Install Windows 11 Pro








