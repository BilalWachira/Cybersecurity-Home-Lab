# Cybersecurity Home Lab

## Overview

This repository documents the development of my personal enterprise-style cybersecurity home lab.

The lab is designed to help me gain practical experience with virtualization, Windows Server, Active Directory, networking, Windows administration, Linux, security monitoring and Governance, Risk and Compliance concepts.

The environment is based on a fictional organisation called **TechSolutions Pty Ltd**.

---

## Current Lab Environment

### Host Computer

- HP ProBook 450 G6
- Intel Core i5-8265U
- 16 GB RAM
- Windows 11 Pro
- Oracle VM VirtualBox
- Virtual machines stored on the D: drive

### Virtual Machines

| Virtual Machine | Operating System | Purpose | Status |
|---|---|---|---|
| TS-DC01 | Windows Server 2022 | Domain Controller, DNS and DHCP | Configuration in progress |
| TS-PC01 | Windows 11 | Simulated employee workstation | Planned |
| TS-SEC01 | Kali Linux | Security testing workstation | Planned |

---

## Completed Work

- Installed Oracle VM VirtualBox
- Created an organised CyberLab folder structure
- Downloaded Windows Server 2022, Windows 11 and Kali Linux ISO files
- Verified that the downloaded files were ISO images
- Configured the VirtualBox default machine folder
- Designed the TS-DC01 virtual machine
- Allocated 4096 MB RAM
- Allocated 2 virtual CPUs
- Created a 60 GB dynamically allocated virtual disk

---

## Lab Roadmap

- [x] Install Oracle VM VirtualBox
- [x] Download operating system ISO files
- [x] Design TS-DC01
- [ ] Install Windows Server 2022
- [ ] Configure Active Directory Domain Services
- [ ] Configure DNS
- [ ] Configure DHCP
- [ ] Create users and groups
- [ ] Configure Group Policy
- [ ] Install Windows 11 client
- [ ] Join Windows 11 to the domain
- [ ] Install Kali Linux
- [ ] Configure security monitoring
- [ ] Create network diagrams

---

## Repository Structure

```text
Cybersecurity-Home-Lab/
├── README.md
├── 01-Planning/
├── 02-VirtualBox/
├── 03-Windows-Server/
├── 04-Active-Directory/
├── 05-DNS/
├── 06-DHCP/
├── 07-Group-Policy/
├── 08-Windows-11/
├── 09-Kali-Linux/
├── 10-Networking/
├── Screenshots/
├── Network-Diagrams/
└── Lessons-Learned/
