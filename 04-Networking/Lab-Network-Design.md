# Home Lab Network Design

## Objective

Create an isolated enterprise-style network that supports Active Directory, Windows clients and security testing while allowing temporary internet access for system updates.

## Network Architecture

The lab uses two VirtualBox networking modes:

### Host-Only Network

The Host-only network provides permanent communication between the host computer and the virtual machines.

Network:

`192.168.56.0/24`

| Device | IP Address |
|---|---|
| VirtualBox Host Adapter | 192.168.56.1 |
| TS-DC01 | 192.168.56.10 |
| TS-PC01 | 192.168.56.20 |
| TS-SEC01 | 192.168.56.30 |

### NAT

A temporary NAT adapter provides internet access for Windows updates and software installation.

The NAT adapter will be disabled before TS-DC01 is promoted to a Domain Controller to avoid multi-homed Domain Controller and DNS-registration issues.

## TS-DC01 Permanent Configuration

| Setting | Value |
|---|---|
| IP Address | 192.168.56.10 |
| Subnet Mask | 255.255.255.0 |
| Default Gateway | None |
| Preferred DNS | 192.168.56.10 |

## Security and GRC Relevance

This design supports:

- Network segmentation
- Controlled internet access
- Stable identity infrastructure
- Configuration management
- Asset documentation
- Reduced exposure of internal lab systems

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
