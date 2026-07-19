# Secure Enterprise & Branch Network Infrastructure Design

## Overview
This project is a Cisco Packet Tracer simulation of a secure multi-site enterprise network. The design includes an Enterprise Headquarters, a remote Branch Office, a routed WAN/core backbone, departmental VLAN segmentation, server infrastructure, centralized services, redundancy mechanisms, and secure management features.

The project was developed as a Computer Networking final project and demonstrates practical CCNA-level networking, infrastructure design, and cybersecurity foundation concepts.

## Project Scope
The network follows a three-tier hierarchical design:

- Core/Edge Layer: WAN/core routers connecting the Enterprise and Branch sites.
- Distribution Layer: Multilayer switches handling inter-VLAN routing and gateway redundancy.
- Access Layer: Access switches providing department-based user connectivity.

## Key Features
- Multi-site Enterprise and Branch network topology
- Department-based VLAN segmentation
- Structured IP addressing and subnetting
- OSPF Area 0 dynamic routing
- HSRP gateway redundancy
- EtherChannel uplink aggregation
- Static NAT for external web server access
- AAA/TACACS+ authentication
- SSH v2 remote management
- DHCP server with multiple VLAN scopes
- FTP server for file sharing and configuration backup
- NTP server for time synchronization
- HTTP/HTTPS web server access
- End-to-end connectivity testing using ping and traceroute

## VLAN Design
| Site | Department | VLAN | Subnet |
|---|---|---:|---|
| Enterprise | HR | 10 | 192.168.10.0/27 |
| Enterprise | Finance | 20 | 192.168.10.32/27 |
| Enterprise | Managers | 30 | 192.168.10.64/27 |
| Enterprise | IT | 40 | 192.168.10.96/28 |
| Enterprise | Servers | 50 | 192.168.10.112/28 |
| Branch | HR | 60 | 192.168.10.128/28 |
| Branch | Finance | 70 | 192.168.10.144/28 |
| Branch | Managers | 80 | 192.168.10.160/28 |
| Branch | IT | 90 | 192.168.10.176/28 |

## Technologies & Concepts
- Cisco Packet Tracer
- VLANs and trunking
- Inter-VLAN routing
- OSPF
- HSRP
- EtherChannel
- LACP and PAgP
- NAT
- AAA/TACACS+
- SSH
- DHCP
- FTP
- NTP
- HTTP/HTTPS
- Network segmentation
- Subnetting
- Network troubleshooting

## Cybersecurity Relevance
This project supports cybersecurity learning by demonstrating the network infrastructure foundations required for SOC analysis, network security monitoring, SIEM investigation, and secure infrastructure administration.

The design applies segmentation, secure remote management, centralized authentication, service isolation, NAT, and connectivity verification. These concepts are important for understanding how enterprise networks are structured, monitored, and secured.

## Verification
The project includes connectivity tests such as:

- Enterprise-to-Branch ping testing
- Internal access to external web server through NAT
- Traceroute path analysis through the OSPF backbone

## Repository Contents
- `Final project.pkt` — Cisco Packet Tracer simulation file
- `Final Project Report.pdf` — Full project documentation
- `topology.png` — Full network topology diagram
- `README.md` — Project overview and technical explanation

## Notes
This is an academic simulation project created for learning and portfolio demonstration. Any lab credentials or shared secrets shown in documentation should be treated as placeholders and should not be reused in real environments.
