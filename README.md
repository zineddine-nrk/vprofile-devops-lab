# VProfile - DevOps Multi-VM Project

Ce projet est une reproduction complète du déploiement de l'application **VProfile**, une application web multi-tier utilisée comme exercice DevOps pour apprendre la mise en place d'infrastructures réalistes.

L’objectif est de déployer manuellement l’application, puis d’automatiser l’ensemble avec des scripts Vagrant et Shell.

---

##  Architecture du projet

L’infrastructure est composée de **5 machines virtuelles**, chacune ayant un rôle spécifique :

- **Nginx (web01)** : Reverse Proxy / Load Balancer  
- **Tomcat (app01)** : Serveur applicatif Java  
- **MySQL (db01)** : Base de données  
- **Memcached (mc01)** : Système de cache distribué  
- **RabbitMQ (rmq01)** : Message broker

L'application Java est compilée avec **Maven**, puis déployée sur **Tomcat**.

---

##  Ce que j'ai appris dans ce projet

### ✔️ Déploiement manuel
- Création de machines virtuelles avec **Vagrant**
- Installation et configuration de :
  - MySQL (MariaDB)
  - Memcached
  - RabbitMQ
  - Tomcat
  - Nginx
- Compilation de l’application avec **Maven**
- Déploiement d’un fichier `.war` dans Tomcat

### ✔️ Automatisation
- Création de scripts Shell pour automatiser l’installation
- Provisioning automatique via **Vagrant**
- Déploiement complet via `vagrant up`

---

## 📦 Technologies utilisées

- **Vagrant**
- **VirtualBox**
- **Linux**
- **MySQL / MariaDB**
- **Memcached**
- **RabbitMQ**
- **Tomcat**
- **Nginx**
- **Maven**
- **Git**

---
