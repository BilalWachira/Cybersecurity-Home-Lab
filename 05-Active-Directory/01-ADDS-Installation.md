# Active Directory Domain Services Installation

## Objective

Install Active Directory Domain Services (AD DS) on TS-DC01 and prepare the server for promotion to a Domain Controller.

## Environment

| Component | Configuration |
|---|---|
| Server | TS-DC01 |
| Operating System | Windows Server 2022 |
| Internal IPv4 Address | 192.168.56.10 |
| Subnet Mask | 255.255.255.0 |
| Preferred DNS | 192.168.56.10 |
| Internal Network | VirtualBox Host-Only |
| Internet/NAT Adapter | Disabled during AD DS deployment |

## Installation

1. Opened Server Manager.
2. Selected **Manage > Add Roles and Features**.
3. Selected **Role-based or feature-based installation**.
4. Selected **TS-DC01** from the server pool.
5. Selected **Active Directory Domain Services**.
6. Added the required AD DS management features.

## Current Status

AD DS role installation in progress.
