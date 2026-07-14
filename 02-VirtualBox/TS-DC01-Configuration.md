# TS-DC01 Virtual Machine Configuration

## Purpose

TS-DC01 will become the first Domain Controller in the fictional TechSolutions Pty Ltd enterprise environment.

## Naming Convention

- `TS` represents TechSolutions
- `DC` represents Domain Controller
- `01` identifies the first server of this type

## Virtual Machine Configuration

| Setting | Value |
|---|---|
| Name | TS-DC01 |
| Operating System | Windows Server 2022 Evaluation |
| Architecture | 64-bit |
| Memory | 4096 MB |
| Processors | 2 vCPUs |
| Virtual Disk | 60 GB |
| Disk Allocation | Dynamically allocated |
| EFI | Disabled |
| Installation Type | Manual installation |

## Configuration Rationale

### Memory

Four gigabytes of memory provides sufficient capacity for Windows Server 2022 and future Active Directory, DNS and DHCP services without consuming excessive host resources.

### Processors

Two virtual CPUs provide suitable lab performance while leaving sufficient processing capacity for Windows 11 and the host operating system.

### Storage

A 60 GB dynamically allocated virtual disk provides room for the operating system, logs and server roles while using physical storage only as needed.

## GRC Relevance

Documenting this configuration supports:

- Asset management
- Configuration management
- Change management
- Capacity planning
- Audit evidence
- Operational risk management
