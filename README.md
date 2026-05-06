# 🌐 Virtual Network Infrastructure with OPNsense

## 📌 Project Overview

This project demonstrates the design and implementation of a virtualized network infrastructure simulating a small enterprise environment.

The goal is to apply core networking concepts such as segmentation, IP addressing, DHCP configuration, and firewall management using a real-world approach.

---

## 🎯 Objectives

* Design a segmented network architecture
* Implement logical separation (ADMIN / USER / GUEST)
* Configure DHCP services for dynamic IP allocation
* Deploy and manage a firewall (OPNsense)
* Simulate enterprise-level network behavior

---

## 🧱 Architecture

The network is divided into three logical segments:

| Network | Role           | Subnet          |
| ------- | -------------- | --------------- |
| ADMIN   | Administration | 192.168.10.0/24 |
| USER    | Employees      | 192.168.20.0/24 |
| GUEST   | Visitors       | 192.168.30.0/24 |

---

## ⚙️ Technologies Used

* OPNsense (Firewall)
* VMware Workstation (Virtualization)
* Windows 10 (Admin client)
* Ubuntu Linux (User client)
* Fedora Linux (Guest client)

---

## 🔧 Implementation Details

### Network Setup

* WAN interface configured with NAT
* LAN interface used for internal communication
* Multiple virtual networks created to simulate VLAN segmentation

### DHCP Configuration

Each segment has its own DHCP scope:

* ADMIN: 192.168.10.100 – 192.168.10.200
* USER: 192.168.20.100 – 192.168.20.200
* GUEST: 192.168.30.100 – 192.168.30.200

---

## 🔐 Security Concept

The architecture is designed to enforce isolation between network segments:

* ADMIN network has full access
* USER and GUEST networks are logically isolated
* Network segmentation inspired by VLAN (802.1Q)

---

## 🧪 Testing

* DHCP assignment verified ✔️
* Connectivity to firewall confirmed ✔️
* Network segmentation behavior partially validated ⚠️

---

## ⚠️ Limitations

* VLANs simulated (no physical switch)
* Advanced firewall rules not fully validated
* No IDS/IPS implemented

---

## 🚀 Future Improvements

* Implement VLAN tagging with managed switch
* Add VPN access
* Deploy IDS/IPS (Snort/Suricata)
* Add monitoring tools (Zabbix / Grafana)

---

## 👨‍💻 Author

Network & Cloud Enthusiast
Aspiring Network Administrator / AWS Cloud Engineer
