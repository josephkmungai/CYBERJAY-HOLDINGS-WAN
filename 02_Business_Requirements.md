# Business Requirements

## Functional Requirements

The network shall:

* Connect the Nairobi Headquarters with the Mombasa, Kisumu, and Tokyo branches.
* Support secure communication between all sites over the WAN.
* Provide centralized authentication and management using Windows Server 2019.
* Allow secure access to enterprise resources from every branch.
* Support dynamic routing using OSPF.
* Provide Internet connectivity through the Nairobi Headquarters.
* Support future branch expansion without redesigning the existing network.
* Separate departments using Virtual LANs (VLANs).
* Allocate IPv4 addresses efficiently using Variable Length Subnet Masking (VLSM).

---

## Non-Functional Requirements

The network shall provide:

* High availability.
* Scalability.
* Redundancy.
* Fault tolerance.
* High performance.
* Centralized management.
* Secure access control.
* Easy maintenance.
* Fast convergence after link failures.

---

## Network Design Requirements

* Cisco hierarchical network architecture.
* Dedicated Core, Distribution, and Access layers.
* Layer 3 switching at Headquarters.
* Layer 2 access switching at each department.
* Redundant WAN connectivity between sites.
* Dedicated Server VLAN.
* Dedicated Management VLAN.
* IEEE 802.1Q trunking between switches.
* Inter-VLAN routing at Headquarters.

---

## Security Requirements

* Access Control Lists (ACLs).
* Secure remote management using SSH.
* Department isolation using VLANs.
* Centralized authentication services.
* Least privilege network access.
* Device management through a dedicated Management VLAN.

---

## Future Expansion

The design allows for:

* Additional branches.
* Additional VLANs.
* IPv6 implementation.
* Wireless LAN integration.
* Cloud service integration.
* VoIP deployment.
* Network monitoring systems.
* Disaster recovery solutions.
