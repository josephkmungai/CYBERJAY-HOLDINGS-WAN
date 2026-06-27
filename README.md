# CYBERJAY-HOLDINGS-WAN

# CyberJay Holdings Enterprise WAN Infrastructure

## Project Overview

CyberJay Holdings Enterprise WAN Infrastructure is a professional enterprise network design project developed to simulate a real-world multi-site technology company. The project demonstrates enterprise networking concepts including Wide Area Network (WAN) design, hierarchical network architecture, VLAN implementation, Variable Length Subnet Masking (VLSM), dynamic routing, Windows Server integration, network security, redundancy, and centralized network management.

The network connects the company's Headquarters in Nairobi with regional branches in Mombasa, Kisumu, and an international procurement branch in Japan. The design follows Cisco Enterprise Campus Network Architecture and industry best practices to provide scalability, redundancy, security, and high availability.

---

## Company Profile

**Company Name:** CyberJay Holdings

**Industry:** Information Technology and Network Solutions

**Headquarters:** Nairobi, Kenya

**Branches:**

* Mombasa, Kenya
* Kisumu, Kenya
* Tokyo, Japan

CyberJay Holdings provides professional services including:

* Enterprise Network Design
* Cybersecurity Solutions
* Network Infrastructure Deployment
* Managed IT Services
* Software Development
* Enterprise Hardware Supply
* Technical Support and Maintenance
* Cloud Integration Services

The Japan branch manages supplier relationships, hardware procurement, product testing, and logistics for networking equipment and enterprise technology solutions.

---

## Project Objectives

The primary objectives of this project are to:

* Design a scalable Enterprise Wide Area Network (WAN).
* Implement Cisco's three-layer hierarchical network model.
* Connect multiple branch offices using dynamic routing.
* Apply Variable Length Subnet Masking (VLSM) for efficient IPv4 allocation.
* Implement VLAN segmentation for improved security and performance.
* Configure centralized services using Windows Server 2019.
* Secure the network using Access Control Lists (ACLs).
* Implement OSPF as the enterprise routing protocol.
* Provide network redundancy and high availability.
* Simulate a real enterprise infrastructure suitable for professional portfolio presentation.

---

## Technologies Used

* Cisco Packet Tracer
* Cisco IOS
* Windows Server 2019
* IPv4 Addressing
* Variable Length Subnet Masking (VLSM)
* VLANs
* IEEE 802.1Q Trunking
* Inter-VLAN Routing
* OSPF
* DHCP
* DNS
* Active Directory Domain Services (AD DS)
* File Services
* Access Control Lists (ACLs)
* SSH Remote Management

---

## Enterprise Network Architecture

The infrastructure follows Cisco's hierarchical network design consisting of:

* Core Layer
* Distribution Layer
* Access Layer

Each branch contains dedicated distribution and access switches while Headquarters hosts the Core Switch, Data Centre, Internet Gateway, and centralized enterprise services.

---

## Repository Structure

```text
cyberjay-holdings-wan/
│
├── README.md
├── 01_Project_Overview.md
├── 02_Business_Requirements.md
├── 03_Network_Architecture.md
├── 04_Device_Inventory.md
├── 05_IP_Addressing_and_VLSM.md
│
├── docs/
│   ├── diagrams/
│   ├── screenshots/
│   └── topology.png
│
├── packet-tracer/
│   └── CyberJay-Holdings-WAN.pkt
│
└── windows-server/
    └── (Configuration files will be added later)
```

---

## Author

**Joseph K. Mungai**

Diploma in Computer Network & System Administration

Cybersecurity Student

---

## Project Status

**Current Phase:** Enterprise Network Planning

Completed:

* Business Requirements
* Branch Structure
* Device Selection
* WAN Topology Planning
* VLAN Planning
* Enterprise VLSM Planning (In Progress)

Upcoming:

* IP Address Allocation
* VLAN Configuration
* Inter-VLAN Routing
* OSPF Configuration
* Windows Server 2019 Deployment
* Enterprise Security Implementation
* Testing and Validation

---

## License

This repository is intended for educational purposes, enterprise networking practice, and professional portfolio demonstration.
