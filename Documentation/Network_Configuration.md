# Network Configuration

## 1. Setting Up Network Interfaces in VMware
- Open VMware settings for the VMs.
- Configure virtual network adapters (e.g., use NAT or bridged networking).

## 2. Configuring Static IP Addresses
- Assign static IPs to both the server and clients.
- Example:
  - Server IP: `192.168.1.10`
  - Client IP: `192.168.1.20`

## 3. Configuring DNS and DHCP
- Use the **DNS Manager** in Windows Server to set up DNS.
- Set up DHCP to assign IP addresses to the client machines automatically (if necessary).

## 4. Network Troubleshooting Tools
- Use `ping`, `tracert`, and `nslookup` to test network connectivity between the server and clients.
