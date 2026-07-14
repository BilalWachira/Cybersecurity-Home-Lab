# Home Lab Hardware

## Host Laptop

| Component | Specification |
|---|---|
| Manufacturer | HP |
| Model | ProBook 450 G6 |
| Processor | Intel Core i5-8265U |
| Physical Cores | 4 |
| Logical Processors | 8 |
| Installed Memory | 16 GB |
| Operating System | Windows 11 Pro |
| System Architecture | 64-bit |

## Storage

| Drive | Total Capacity | Available Space | Use |
|---|---:|---:|---|
| C: | Approximately 277 GB | Approximately 50 GB | Host operating system |
| D: | Approximately 197 GB | Approximately 192 GB | Cybersecurity home lab |

## Resource Planning

Virtual machines are stored on the D: drive to avoid filling the host operating system drive.

The initial TS-DC01 server configuration uses:

- 4096 MB RAM
- 2 virtual CPUs
- 60 GB dynamically allocated virtual storage

This allocation provides sufficient resources for Windows Server 2022 while leaving enough memory and CPU capacity for the host computer.
