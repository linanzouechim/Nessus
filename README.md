🛡️ Scan de vulnérabilités avec Nessus
Analyse de Metasploitable 2 depuis Kali Linux

📌 Description du projet
Ce laboratoire pratique a été réalisé dans le cadre de ma formation en cybersécurité.
L’objectif était de mettre en place un environnement contrôlé, d’y installer Nessus Essentials sur une machine Kali Linux, puis d’effectuer un scan de vulnérabilités complet sur une machine cible Metasploitable 2, volontairement vulnérable.

Ce projet démontre ma capacité à :

Configurer un outil de gestion des vulnérabilités (Nessus)

Identifier, analyser et prioriser des failles de sécurité

Interpréter les résultats et proposer des mesures correctives

Travailler dans un environnement virtualisé et isolé

🧰 Environnement utilisé
Composant	Détails
Machine d’analyse	Kali Linux (VM)
Outil de scan	Nessus Essentials
Machine cible	Metasploitable 2
Hyperviseur	VMware / VirtualBox
Réseau	NAT ou Host‑Only selon configuration
🚀 Étapes réalisées
1. Installation et configuration de Nessus
Téléchargement de Nessus Essentials depuis Tenable

Installation sur Kali Linux

Activation via clé d’enregistrement

Mise à jour des plugins de détection

Configuration de l’interface Web (port 8834)

2. Préparation de l’environnement
Démarrage de Metasploitable 2

Vérification de la connectivité réseau (ping, nmap)

Identification de l’adresse IP cible

3. Création et lancement du scan
Création d’un Basic Network Scan

Définition de la cible : IP de Metasploitable 2

Paramétrage des options (port scan, authentification, intensité)

Lancement du scan et suivi en temps réel

4. Analyse des résultats
Nessus a détecté plusieurs vulnérabilités critiques, notamment :

Services obsolètes (vsftpd, Apache, OpenSSH)

Ports ouverts non sécurisés

Vulnérabilités connues (CVE) exploitables

Failles liées à MySQL, RPC, Telnet, Samba

Mauvaises configurations et mots de passe par défaut

5. Recommandations proposées
Mise à jour des services et paquets

Désactivation des services inutiles

Renforcement des configurations SSH / FTP

Application de correctifs de sécurité

Segmentation réseau et durcissement du système

📊 Résultats (exemples)
⚠️ Aucun résultat sensible n’est publié — uniquement des extraits pédagogiques.

Nombre total de vulnérabilités détectées : 60+

Critiques : 10

Élevées : 15

Moyennes : 20

Faibles : 15

📚 Compétences développées
Gestion des vulnérabilités

Analyse de rapports Nessus

Interprétation des CVE

Évaluation des risques

Mise en place d’un environnement de test sécurisé

Méthodologie SOC / Blue Team


📝 Conclusion
Ce laboratoire m’a permis de comprendre en profondeur le fonctionnement d’un scan de vulnérabilités, d’interpréter les résultats générés par Nessus et de proposer des mesures de mitigation adaptées.
Il constitue une base solide pour mes futurs projets en cyberdéfense, gestion des vulnérabilités et analyse SOC.
