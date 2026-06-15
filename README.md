# 🌐 Multi-Site Enterprise Network Design

<p align="center">
  <img src="https://img.shields.io/badge/Tool-Cisco%20Packet%20Tracer-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white" />
  <img src="https://img.shields.io/badge/Protocol-OSPF%20%7C%20EIGRP-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white" />
  <img src="https://img.shields.io/badge/Service-VPN%20%7C%20WAN-4B4B4B?style=for-the-badge&logo=cisco&logoColor=white" />
  <img src="https://img.shields.io/badge/Architecture-Multi--Site%20Enterprise-E22C2C?style=for-the-badge&logo=target&logoColor=white" />
</p>

> 🏢 A fully simulated multi-branch enterprise WAN connecting geographically distributed offices using dynamic routing, inter-site VPN tunnels, VLAN segmentation, and redundant connectivity — built in Cisco Packet Tracer.

---

## 📌 Overview

This project designs and implements a **multi-site enterprise network** connecting multiple branch offices to a central headquarters over a simulated WAN. The design incorporates dynamic routing protocols, secure site-to-site VPN tunnels, VLAN-based segmentation, and redundancy mechanisms to reflect real-world enterprise WAN architecture.

---

## 🏗️ Network Architecture

### Network Diagram

<img width="2562" height="1016" alt="image" src="https://github.com/user-attachments/assets/c3b87fda-4b71-43ff-93a0-c589abc687f2" />

### Sites

| Site | Role |
|------|------|
| Headquarters (HQ) | Central hub — hosts core services and internet gateway |
| Branch Office 1 | Remote site connected via WAN |
| Branch Office 2 | Remote site connected via WAN |

### Design Principles
- **Hierarchical design** — Core, Distribution, and Access layers
- **Redundant links** — no single point of failure between sites
- **Segmented VLANs** — per-department traffic isolation at each site
- **Centralized internet access** — all branch traffic routed through HQ

---

## 🛠️ Technologies Implemented

### 🔄 Routing & WAN
- **OSPF** — dynamic routing between HQ and branch sites
- **EIGRP** — internal routing within site boundaries
- **Static routing** — fallback and specific route configuration
- **WAN simulation** — serial links connecting geographically distributed sites

### 🔒 Security & VPN
- **Site-to-site VPN tunnels** — encrypted inter-branch communication
- **ACLs** — traffic filtering between sites and internet
- **SSH** — secure remote management across all devices

### 🌐 Network Services
- **VLANs** — department-level segmentation at each site
- **Inter-VLAN routing** — Layer 3 switching
- **DHCP** — dynamic IP assignment per VLAN per site
- **NAT/PAT** — internet access for all branch users via HQ
- **NTP** — synchronized time across all devices

### 📡 Redundancy
- **EtherChannel** — aggregated uplinks between distribution and core switches
- **HSRP/STP** — gateway redundancy and loop prevention
- **Dual WAN links** — failover between primary and backup ISP connections

---

## 🔑 Key Accomplishments

- ✅ Connected multiple geographically distributed sites over a simulated WAN
- ✅ Configured OSPF dynamic routing for automatic route propagation between sites
- ✅ Implemented encrypted site-to-site VPN tunnels for secure inter-branch traffic
- ✅ Designed VLAN hierarchy at each site for department-level isolation
- ✅ Enabled internet access for all branches via centralized NAT at HQ
- ✅ Configured redundant WAN links with failover capability
- ✅ Applied ACLs to enforce traffic policies between sites

---

## 🗺️ High-Level Topology

```
         [ISP / Internet]
                |
         [HQ Core Router]
          /           \
    [HQ Dist SW]    [WAN Links]
         |            /      \
    [HQ Access]  [Branch 1]  [Branch 2]
                  Router       Router
                    |            |
                 [SW B1]      [SW B2]
                VLANs          VLANs
```

---

## 📋 Implementation Steps

| Step | Task |
|------|------|
| 1 | Network topology design and IP addressing plan |
| 2 | HQ core and distribution layer setup |
| 3 | Branch office switch and router configuration |
| 4 | WAN serial link configuration between sites |
| 5 | OSPF dynamic routing configuration |
| 6 | VLAN creation and inter-VLAN routing at each site |
| 7 | DHCP configuration per VLAN per site |
| 8 | Site-to-site VPN tunnel configuration |
| 9 | NAT/PAT for internet access via HQ |
| 10 | ACL enforcement between zones |
| 11 | Redundancy — EtherChannel, HSRP, STP |
| 12 | End-to-end connectivity testing and verification |

---

## 📁 Repository Contents

```
📦 Multi-Site-Enterprise-Network
├── 📄 README.md
└── 📋 Project Report.pdf    ← Full design report and topology diagrams
```

---

## 🧠 Skills Demonstrated

`OSPF` `EIGRP` `Site-to-Site VPN` `WAN Design` `VLAN Segmentation` `NAT/PAT` `ACL` `EtherChannel` `HSRP` `Spanning Tree` `Enterprise Network Design` `Cisco Packet Tracer` `Network Redundancy` `Multi-Site Architecture`

---

## 💡 Real-World Relevance

Multi-site enterprise networks are the backbone of corporate IT infrastructure. This project demonstrates skills directly applicable to:
- **Network Engineer** roles — WAN design, routing protocol configuration
- **Security Engineer** roles — VPN, ACL, and zone-based security
- **SOC Analyst** roles — understanding traffic flow for threat detection
- **PhD research** — network architecture and security policy enforcement at scale

---

## ⚠️ Disclaimer

This project was designed and implemented in Cisco Packet Tracer for academic and educational purposes. All company names, IP addresses, and configurations are fictitious.

---

## 👤 Author

**Hashan Kodippilige**  
M.S. Cybersecurity — Minnesota State University Moorhead  
📧 hashansharindu@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/hashankodippilige/)  
🐙 [GitHub](https://github.com/hashan-kodippilige)
