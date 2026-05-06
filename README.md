# network-project-opnsense
Virtual Network Infrastructure with OPNsense
# 🖧 Projet Infrastructure Réseau & Cloud – Administration Systèmes

## 📌 Présentation
Ce projet simule une infrastructure réseau d’entreprise moderne intégrant :
- Administration Windows 10 / Windows Server
- Segmentation VLAN
- Sécurité réseau (Firewall, ACL)
- Services réseau (DNS, DHCP, Active Directory)
- Intégration Cloud (AWS / VPN Site-to-Site)

---

## 🏗️ Architecture

L’infrastructure est composée de :

- 🌐 Internet (ISP)
- 🔥 Firewall (OPNsense)
- 🖧 Switch L2/L3 (VLANs)
- 🖥️ Serveur Windows (AD DS, DNS, DHCP)
- 👨‍💻 Clients Windows 10
- ☁️ AWS (optionnel : VPC, EC2, VPN)

---

## 🔐 Segmentation VLAN

| VLAN | Description        | Sous-réseau        |
|------|------------------|--------------------|
| 10   | Administration    | 192.168.10.0/24    |
| 20   | Utilisateurs      | 192.168.20.0/24    |
| 30   | Serveurs          | 192.168.30.0/24    |
---

## ⚙️ Services configurés

### 🖥️ Active Directory
- Gestion centralisée des utilisateurs
- Politique de groupe (GPO)

### 🌐 DNS / DHCP
- Résolution de noms interne
- Attribution automatique des IP

### 🔥 Sécurité réseau
- Règles firewall (filtrage entrant/sortant)
- NAT/PAT
- Isolation VLAN

---

## 🚀 Technologies utilisées
- Windows Server 2019/2022
- Windows 10
- Cisco / Virtual Switch
- OPNsense
- AWS (EC2, VPC, VPN)
- VMware / VirtualBox

---

## 📊 Objectifs du projet
- Concevoir une architecture réseau professionnelle
- Sécuriser les flux internes et externes
- Simuler un environnement entreprise réel
- Préparer certification CCNA / AWS Practitioner

---

## 👨‍💻 Auteur
Administrateur Systèmes & Réseaux (Junior)
