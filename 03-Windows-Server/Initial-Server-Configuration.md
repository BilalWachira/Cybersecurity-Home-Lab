# Initial Server Configuration

## Initial Review

After installing Windows Server 2022, I reviewed the default configuration using Server Manager.

### Findings

- Computer Name: WIN-4ODHLB72MU6
- Workgroup: WORKGROUP
- Firewall: Enabled
- Remote Management: Enabled
- Remote Desktop: Disabled
- Network Configuration: DHCP
- Windows Defender: Enabled
- Time Zone: Pacific Time (US & Canada)

### Planned Changes

- Rename server to TS-DC01
- Configure Australian Eastern Standard Time
- Assign a static IPv4 address
- Prepare the server for Active Directory Domain Services (AD DS)

## Server Renaming

### Original Name

WIN-4ODHLB72MU6

### New Name

TS-DC01

### Reason

Enterprise environments use standardized naming conventions to make servers easier to identify, manage and document.

For this lab, the naming convention is:

- TS = TechSolutions
- DC = Domain Controller
- 01 = First Domain Controller

## Completed Initial Configuration

- Renamed server to TS-DC01
- Configured Australian time zone
- Assigned static IPv4 address (192.168.56.10)
- Configured preferred DNS to self (192.168.56.10)
- Restarted the server to apply configuration changes

Status: Ready for Active Directory Domain Services installation.
