# Week 3 – Enterprise Server Deployment and Operating System Installation

**Program:** BSIT | **Course:** ITEP 414 – System Administration and Maintenance
**Role:** Junior System Administrator, ABC Startup Solutions

## Project Overview
This project deploys Ubuntu Server as the company's first Linux server, to be used for
file sharing, remote administration, database hosting, web hosting, and internal services.
It covers installation, configuration, verification, and comparison of boot technologies
and enterprise operating systems.

## Learning Objectives
- Explain the purpose of an OS in enterprise environments
- Differentiate BIOS and UEFI firmware
- Explain the stages of the computer boot process
- Compare Ubuntu Server, Windows Server, and Rocky Linux
- Install and configure Ubuntu Server in a VM
- Enable and verify SSH for remote administration

## Virtual Machine Specifications
| Component | Value |
|---|---|
| Name | Ubuntu-Server-Week03 |
| RAM | 4 GB |
| CPU | 2 vCPUs |
| Storage | 40 GB (VDI/VMDK) |
| Network | NAT |
| Optical Drive | Ubuntu Server LTS ISO |

## Installation Summary
<!-- TODO: Fill in after installation -->
- Hostname: `server01`
- Username: `<yourlastname>`
- Assigned IP address (from `ip addr`): `<fill in>`
- Disk partition scheme / filesystem used: `<fill in>`

## Configuration Summary
<!-- TODO -->
- SSH: OpenSSH Server installed during setup
- Additional packages installed: none (per instructions)

## Verification Results
| Task | Command | Result |
|---|---|---|
| Login | — | ☐ Verified |
| Hostname | `hostname` | ☐ Verified |
| IP Address | `ip addr` | ☐ Verified |
| Internet Connectivity | `ping -c 4 google.com` | ☐ Verified |
| System Update | `sudo apt update && sudo apt upgrade -y` | ☐ Verified |
| SSH Service | `systemctl status ssh` | ☐ active (running) |

*(Attach screenshots for each task in `/screenshots`.)*

## BIOS vs UEFI Highlights
See `BIOS_vs_UEFI.docx` for the full comparison. Key takeaway: UEFI has replaced BIOS
in modern enterprise environments due to support for disks larger than 2 TB, Secure
Boot, faster parallel initialization, and GPT's 128-partition support versus MBR's 4.

## Boot Process Flowchart
![Ubuntu Boot Process](diagrams/BootProcessFlowchart.png)

## Challenges Encountered
<!-- TODO: Fill in based on your actual installation experience, e.g. network
adapter issues, disk partition prompts, SSH not enabling by default, etc. -->

## Reflection (300–500 words)
<!-- TODO: Write your personal reflection here covering what you learned about
Ubuntu Server deployment, why BIOS/UEFI knowledge matters for a sysadmin, and
how this exercise connects to real enterprise practice. -->

## References
- Ubuntu Server Documentation – https://ubuntu.com/server/docs
- Red Hat / Rocky Linux Documentation – https://docs.rockylinux.org
- Microsoft Windows Server Documentation – https://learn.microsoft.com/windows-server/
- UEFI Specification – https://uefi.org/specifications
