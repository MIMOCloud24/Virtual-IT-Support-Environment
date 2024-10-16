# Setup Instructions

## 1. Setting Up VMware Environment
### 1.1. Install VMware Workstation Pro
- Download and install VMware Workstation Pro from [VMware's website](https://www.vmware.com/products/desktop-hypervisor/workstation-and-fusion). Choose for personal use option it is free.
- Create virtual machines for Windows Server and Windows clients. (I used Windows server 2022 and Windows 10). You can download windows server 2022 and windows 11 from [Microsoft's website](https://www.microsoft.com/en-us/evalcenter).
### 1.2. Configure VMware Virtual Network
- Set up the virtual network to allow communication between the server and client machines.

## 2. Installing Windows Server
- Install Windows Server 2022 (or another version) on one of the VMs.
- Promote the server to a Domain Controller to enable Active Directory services.

## 3. Installing Windows Clients
- Create VMs for Windows 10 or Windows 11 clients.
