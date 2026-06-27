
# 📌 Project Overview

This project presents the design and implementation of a **Secure IP/MPLS Backbone Network** simulating a real-world Internet Service Provider (ISP) infrastructure.

The entire network was designed, configured, and validated using **GNS3**, combining Cisco networking technologies with enterprise security and management solutions. The objective was to build a scalable, secure, and highly available infrastructure capable of providing MPLS VPN connectivity between multiple customer sites while ensuring centralized authentication, network monitoring, and secure access to public services hosted in a DMZ.

---

# 🛠️ Simulation Environment

The project was entirely implemented and tested using the following environment:

- **GNS3** (Network Simulation Platform)
- Cisco IOS Routers
- Cisco Layer 2 & Layer 3 Switches
- Cisco ASAv Firewalls
- Ubuntu Server
- VMware Workstation

---

# 🏗️ Network Architecture

![Network Topology](Architecture.png)

The architecture is composed of four main modules:

- **IP/MPLS Backbone**
- **Campus Network**
- **AAA, Management & Monitoring**
- **Firewall & DMZ Security**

---

# 🚀 Project Implementation

## ▶ Part 1 & 2 — IP/MPLS Backbone

The first phase focused on building the service provider backbone and connecting multiple customer sites through a secure MPLS VPN infrastructure.

### Implemented Features

- Multi-area OSPF routing (Areas 0, 11, 12, 21 and 22)
- MPLS with LDP label distribution
- MP-BGP for MPLS Layer 3 VPN route exchange
- VRF implementation for customer traffic isolation
- PE, P and CE router architecture
- Inter-VLAN Routing
- VLAN segmentation
- DHCP services for multiple VLANs
- EtherChannel (LACP)
- HSRP / VRRP gateway redundancy

---

## ▶ Part 3 — AAA, Management & Monitoring

A centralized management platform was implemented to improve network administration, monitoring and operational security.

### Implemented Features

- Centralized AAA authentication using FreeRADIUS
- Authentication and Authorization
- User privilege levels (1, 10 and 15)
- Extended ACLs protecting VTY access
- Network monitoring using Zabbix 7.0
- Secure SNMPv3 monitoring
- Centralized Syslog server
- NTP time synchronization
- IP SLA measurements:
  - Latency
  - Jitter
  - Packet Loss

---

## ▶ Part 4 — Firewall & DMZ Security

The enterprise perimeter is protected by redundant Cisco ASAv firewalls, providing secure access to services hosted inside a dedicated DMZ.

### DMZ Services

- 🌐 Apache2 Web Server
- 📧 Postfix SMTP Mail Server
- 🔍 Bind9 DNS Server (dmz.local)

### Security Features

- Cisco ASAv Firewalls (FW1 & FW2)
- Security Zones
- Stateful ACL policies
- HTTP filtering
- SMTP filtering
- DNS filtering
- ICMP filtering
- End-to-end DNS resolution validation

---

# 🛠️ Technologies Used

| Category | Technologies |
|-----------|--------------|
| Network Simulation | GNS3 |
| Routing | OSPF, MPLS, MP-BGP |
| VPN | MPLS Layer 3 VPN, VRF |
| Switching | VLAN, Inter-VLAN Routing, EtherChannel (LACP), HSRP, VRRP |
| Security | Cisco ASAv, ACLs |
| AAA | FreeRADIUS |
| Monitoring | Zabbix 7.0, SNMPv3, IP SLA |
| Management | Syslog, NTP |
| Linux Services | Apache2, Postfix, Bind9 |
| Operating Systems | Cisco IOS, Ubuntu Server |
| Virtualization | VMware Workstation |

---

# 🎯 Skills Demonstrated

- ISP IP/MPLS Network Design
- MPLS Layer 3 VPN Deployment
- Advanced Routing (OSPF & MP-BGP)
- VLAN & Inter-VLAN Routing
- High Availability (HSRP / VRRP)
- AAA Authentication with FreeRADIUS
- Network Monitoring & Performance Analysis
- Cisco ASAv Firewall Configuration
- DMZ Design & Security
- Linux Network Services Administration
- Network Troubleshooting

---

# 📄 Conclusion

This project provided hands-on experience in designing and deploying a complete ISP-grade IP/MPLS infrastructure, combining advanced routing, VPN technologies, high availability, centralized authentication, network monitoring, and perimeter security.

It demonstrates practical knowledge of enterprise networking and cybersecurity concepts commonly used in modern service provider and enterprise environments.
