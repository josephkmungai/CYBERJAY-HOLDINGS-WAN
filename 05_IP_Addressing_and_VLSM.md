# IP Addressing and VLSM

## IPv4 Addressing Scheme

CyberJay Holdings uses the private IPv4 address block **10.0.0.0/8**. Each company location is allocated a dedicated address space to simplify routing, troubleshooting, and future expansion.

| Site                 | Network Block |
| -------------------- | ------------- |
| Nairobi Headquarters | 10.10.0.0/16  |
| Mombasa Branch       | 10.20.0.0/16  |
| Kisumu Branch        | 10.30.0.0/16  |
| Tokyo Branch         | 10.40.0.0/16  |
| WAN Links            | 10.255.0.0/24 |

---

# Nairobi Headquarters

| VLAN | Department               | Network    | CIDR | Gateway    |
| ---- | ------------------------ | ---------- | ---- | ---------- |
| 110  | Administration & Finance | 10.10.10.0 | /24  | 10.10.10.1 |
| 120  | Software Development     | 10.10.20.0 | /24  | 10.10.20.1 |
| 130  | Technical Operations     | 10.10.30.0 | /25  | 10.10.30.1 |
| 140  | Servers                  | 10.10.40.0 | /26  | 10.10.40.1 |
| 499  | Network Management       | 10.10.99.0 | /26  | 10.10.99.1 |

---

# Mombasa Branch

| VLAN | Department | Network    | CIDR | Gateway    |
| ---- | ---------- | ---------- | ---- | ---------- |
| 210  | Sales      | 10.20.10.0 | /25  | 10.20.10.1 |
| 220  | Engineers  | 10.20.20.0 | /25  | 10.20.20.1 |
| 230  | Deployment | 10.20.30.0 | /25  | 10.20.30.1 |

---

# Kisumu Branch

| VLAN | Department | Network    | CIDR | Gateway    |
| ---- | ---------- | ---------- | ---- | ---------- |
| 310  | Sales      | 10.30.10.0 | /25  | 10.30.10.1 |
| 320  | Engineers  | 10.30.20.0 | /25  | 10.30.20.1 |
| 330  | Deployment | 10.30.30.0 | /25  | 10.30.30.1 |

---

# Tokyo Branch

| VLAN | Department               | Network    | CIDR | Gateway    |
| ---- | ------------------------ | ---------- | ---- | ---------- |
| 410  | Administration           | 10.40.10.0 | /25  | 10.40.10.1 |
| 420  | Sales & Vendor Relations | 10.40.20.0 | /24  | 10.40.20.1 |
| 430  | Hardware Engineering     | 10.40.30.0 | /25  | 10.40.30.1 |

---

# WAN Point-to-Point Links

| Link             | Network     | CIDR |
| ---------------- | ----------- | ---- |
| HQ ↔ Mombasa     | 10.255.0.0  | /30  |
| Mombasa ↔ Kisumu | 10.255.0.4  | /30  |
| Kisumu ↔ Tokyo   | 10.255.0.8  | /30  |
| Tokyo ↔ HQ       | 10.255.0.12 | /30  |

---

# Addressing Standards

* The first usable IP address in every subnet is reserved as the default gateway.
* Infrastructure devices receive static IP addresses.
* End-user devices receive IP addresses dynamically through DHCP.
* Servers use static IP addresses.
* WAN links use /30 subnets to conserve IPv4 address space.
* Network addressing follows a hierarchical structure based on site and department.
