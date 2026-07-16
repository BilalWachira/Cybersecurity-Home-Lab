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
