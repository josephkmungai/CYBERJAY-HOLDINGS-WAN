# Network Architecture

## Network Model

The infrastructure follows the Cisco Three-Layer Hierarchical Network Model.

### Core Layer

Located at the Nairobi Headquarters.

Responsibilities:

* High-speed backbone switching
* Inter-VLAN routing
* WAN traffic forwarding
* Route processing
* Redundant path selection

---

### Distribution Layer

Located at every company site.

Responsibilities:

* Aggregates Access Switches
* VLAN boundary enforcement
* Policy implementation
* Traffic forwarding to the Core Layer

---

### Access Layer

Located within each department.

Responsibilities:

* End device connectivity
* VLAN assignment
* Port security
* User access to network resources

---

# WAN Architecture

The enterprise WAN connects all company locations using a redundant ring topology.

```text
                    Nairobi HQ
                   (Core Network)
                   /           \
                  /             \
          Mombasa               Tokyo
                 \             /
                  \           /
                    Kisumu
```

Each branch communicates using OSPF, allowing automatic route recalculation if a WAN link fails.

---

# Internet Architecture

Internet connectivity is centralized at the Nairobi Headquarters.

```text
Internet
    │
ISP Cloud
    │
Edge Router
    │
Firewall
    │
Core Switch
```

All Internet-bound traffic from branch offices passes securely through the Headquarters.

---

# Data Centre

The enterprise data centre is located at the Nairobi Headquarters.

Services include:

* Active Directory Domain Services
* DNS
* DHCP
* File Services
* Network Time Services
* Centralized Authentication
* Shared Storage

---

# Enterprise Design Principles

* Modular architecture
* High availability
* Scalability
* Redundancy
* Centralized management
* Secure segmentation
* Simplified troubleshooting
* Efficient resource utilization
