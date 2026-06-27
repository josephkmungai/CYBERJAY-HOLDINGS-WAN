# Network Topology and Device Placement

## Topology Overview

CyberJay Holdings uses a hierarchical enterprise WAN topology consisting of one Headquarters and three branch offices connected through redundant WAN links.

```text
                          ISP Cloud
                              │
                        Cisco 2911
                         (HQ Router)
                              │
                    Cisco 3650 Core Switch
                              │
      ┌───────────────┬───────────────┬───────────────┐
      │               │               │
  Dist-SW-ADM     Dist-SW-DEV     Dist-SW-TECH
      │               │               │
  Access Switch   Access Switch  Access Switch
      │               │               │
  End Devices     End Devices    End Devices
                              │
                       Windows Server 2019
```

---

# WAN Topology

```text
                    Nairobi HQ
                    /         \
                   /           \
          Mombasa               Tokyo
               \               /
                \             /
                  Kisumu
```

The ring topology provides an alternate communication path if a WAN link becomes unavailable.

---

# Nairobi Headquarters

## Devices

| Device                         |    Quantity |
| ------------------------------ | ----------: |
| Cisco 2911 Router              |           1 |
| Cisco 3650 Core Switch         |           1 |
| Cisco 3650 Distribution Switch |           3 |
| Cisco 2960 Access Switch       |           3 |
| Windows Server 2019            |           1 |
| PCs                            | As Required |
| Printers                       | As Required |

---

# Mombasa Branch

## Devices

| Device                         |    Quantity |
| ------------------------------ | ----------: |
| Cisco 2911 Router              |           1 |
| Cisco 3650 Distribution Switch |           1 |
| Cisco 2960 Access Switch       |           3 |
| PCs                            | As Required |
| Printers                       | As Required |

---

# Kisumu Branch

## Devices

| Device                         |    Quantity |
| ------------------------------ | ----------: |
| Cisco 2911 Router              |           1 |
| Cisco 3650 Distribution Switch |           1 |
| Cisco 2960 Access Switch       |           3 |
| PCs                            | As Required |
| Printers                       | As Required |

---

# Tokyo Branch

## Devices

| Device                         |    Quantity |
| ------------------------------ | ----------: |
| Cisco 2911 Router              |           1 |
| Cisco 3650 Distribution Switch |           1 |
| Cisco 2960 Access Switch       |           3 |
| PCs                            | As Required |
| Printers                       | As Required |

---

# Cabling Standards

| Connection                        | Cable Type                       |
| --------------------------------- | -------------------------------- |
| ISP Cloud ↔ HQ Router             | Copper Straight-Through          |
| Router ↔ Distribution/Core Switch | Copper Straight-Through          |
| Distribution ↔ Access Switch      | Multimode Fiber with SFP Modules |
| Access Switch ↔ PCs               | Copper Straight-Through          |
| Access Switch ↔ Printers          | Copper Straight-Through          |
| Access Switch ↔ Server            | Copper Straight-Through          |

---

# Design Standards

* One router per site.
* One distribution switch per branch.
* Three distribution switches at Headquarters.
* One access switch for each department.
* One centralized server located at Nairobi Headquarters.
* Internet access centralized through the Headquarters.
* Redundant WAN links configured between all sites.
* Structured device placement following Cisco hierarchical design principles.
