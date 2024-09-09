
### Ports 0 à 1023 (Ports bien connus)

20 - FTP (File Transfer Protocol) - Transfert de fichiers (données)
21 - FTP (File Transfer Protocol) - Transfert de fichiers (contrôle)
22 - SSH (Secure Shell) - Connexion à distance sécurisée
23 - Telnet - Connexion à distance non sécurisée
25 - SMTP (Simple Mail Transfer Protocol) - Envoi de courriers électroniques
53 - DNS (Domain Name System) - Résolution des noms de domaine
67/68 - DHCP (Dynamic Host Configuration Protocol) - Attribution d'adresses IP dynamiques (client/serveur)
80 - HTTP (Hypertext Transfer Protocol) - Web (non sécurisé)
110 - POP3 (Post Office Protocol) - Récupération de courriers électroniques
119 - NNTP (Network News Transfer Protocol) - Transfert de nouvelles (Usenet)
123 - NTP (Network Time Protocol) - Synchronisation de l'heure sur le réseau
143 - IMAP (Internet Message Access Protocol) - Gestion et lecture des courriels
161/162 - SNMP (Simple Network Management Protocol) - Gestion de réseaux
389 - LDAP (Lightweight Directory Access Protocol) - Accès aux services d'annuaire
443 - HTTPS (Hypertext Transfer Protocol Secure) - Web sécurisé via SSL/TLS
465 - SMTPS (Simple Mail Transfer Protocol Secure) - Envoi sécurisé de courriels
514 - Syslog - Journalisation d'événements réseau
587 - SMTP (Submission) - Envoi de courriels avec authentification
636 - LDAPS (Lightweight Directory Access Protocol Secure) - Annuaire sécurisé via SSL/TLS
989/990 - FTPS (FTP Secure) - Transfert de fichiers sécurisé via SSL/TLS

### Ports 1024 à 49151 (Ports enregistrés)

1433/1434 - Microsoft SQL Server - Bases de données SQL Server
1521 - Oracle Database - Bases de données Oracle
3306 - MySQL - Bases de données MySQL
3389 - RDP (Remote Desktop Protocol) - Connexion de bureau à distance
5432 - PostgreSQL - Bases de données PostgreSQL
5900 - VNC (Virtual Network Computing) - Bureau à distance VNC
6379 - Redis - Base de données en mémoire Redis
8080 - HTTP alternatif - HTTP non sécurisé sur un port différent

### Ports 49152 à 65535 (Ports dynamiques/privés)

Ces ports sont souvent utilisés pour des connexions temporaires ou des ports éphémères assignés dynamiquement.


## outil :

Pour connaitre les port ouvert d'une machine [[nmap]] est l'outil parfait.

```c
┌──(rihaltun㉿T470-kali)-[~]
└─$ nmap 8.8.8.8             
Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-09-06 22:37 CEST
Nmap scan report for dns.google (8.8.8.8)
Host is up (0.014s latency).
Not shown: 998 filtered tcp ports (no-response)
PORT    STATE SERVICE
53/tcp  open  domain
443/tcp open  https

Nmap done: 1 IP address (1 host up) scanned in 4.90 seconds

┌──(rihaltun㉿T470-kali)-[~]
└─$ 
```


