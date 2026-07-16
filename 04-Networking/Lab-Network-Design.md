## TS-DC01 Network Configuration

The server uses two network adapters:

### Adapter 1 – Host-Only

Purpose:
- Internal enterprise communication
- Active Directory
- DNS
- DHCP
- Windows client communication

Configuration:

- IPv4 Address: 192.168.56.10
- Subnet Mask: 255.255.255.0

### Adapter 2 – NAT

Purpose:
- Temporary internet connectivity
- Windows Updates
- Software installation

Configuration:

- IPv4 Address: Assigned automatically by VirtualBox NAT
