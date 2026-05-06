# 🌐 Infrastructure Réseau Virtualisée avec OPNsense

## 📌 Présentation du projet

Ce projet présente la conception et la mise en œuvre d’une infrastructure réseau virtualisée simulant un environnement d’entreprise (PME).

L’objectif est d’appliquer des concepts fondamentaux en réseau tels que la segmentation, l’adressage IP, la configuration DHCP et la gestion d’un pare-feu, dans un contexte proche du réel.

---

## 🎯 Objectifs

* Concevoir une architecture réseau segmentée
* Mettre en place une séparation logique (ADMIN / USER / GUEST)
* Configurer un service DHCP pour l’attribution dynamique des adresses IP
* Déployer et administrer un pare-feu (OPNsense)
* Simuler un environnement réseau d’entreprise

---

## 🧱 Architecture

Le réseau est divisé en trois segments logiques :

| Réseau | Rôle           | Sous-réseau     |
| ------ | -------------- | --------------- |
| ADMIN  | Administration | 192.168.10.0/24 |
| USER   | Employés       | 192.168.20.0/24 |
| GUEST  | Invités        | 192.168.30.0/24 |

---

## ⚙️ Technologies utilisées

* OPNsense (Pare-feu)
* VMware Workstation (Virtualisation)
* Windows 10 (poste ADMIN)
* Ubuntu Linux (poste USER)
* Fedora Linux (poste GUEST)

---

## 🔧 Détails de l’implémentation

### Configuration réseau

* Interface WAN configurée en NAT (accès Internet simulé)
* Interface LAN utilisée pour la communication interne
* Création de plusieurs réseaux virtuels pour simuler une segmentation de type VLAN

---

### Configuration DHCP

Chaque segment dispose de sa propre plage d’adressage :

* ADMIN : 192.168.10.100 – 192.168.10.200
* USER : 192.168.20.100 – 192.168.20.200
* GUEST : 192.168.30.100 – 192.168.30.200

---

## 🔐 Concept de sécurité

L’architecture a été conçue pour assurer une isolation logique entre les segments réseau :

* Le réseau ADMIN dispose d’un accès complet
* Les réseaux USER et GUEST sont isolés logiquement
* La segmentation s’inspire du principe des VLAN (IEEE 802.1Q)

---

## 🧪 Tests réalisés

* Attribution dynamique des adresses IP (DHCP) validée ✔️
* Connectivité avec le pare-feu vérifiée ✔️
* Comportement de segmentation partiellement validé ⚠️

---

## ⚠️ Limites du projet

* VLAN simulés (absence de switch manageable)
* Règles de pare-feu non entièrement validées
* Absence de système IDS/IPS

---

## 🚀 Améliorations futures

* Implémentation de VLAN réels avec un switch manageable
* Mise en place d’un VPN
* Déploiement d’un IDS/IPS (Snort / Suricata)
* Ajout d’outils de supervision (Zabbix / Grafana)

---

## 👨‍💻 Auteur

Passionné de réseaux et de cloud
Futur Administrateur Réseau / Ingénieur Cloud AWS
