# 🛡️ Scan de vulnérabilités avec Nessus  
Analyse de Metasploitable 2 depuis Kali Linux

## 📌 Description du projet
Ce laboratoire pratique a été réalisé dans le cadre de ma formation en cybersécurité.  
L’objectif était de mettre en place un environnement contrôlé, d’y installer Nessus Essentials sur une machine Kali Linux, puis d’effectuer un scan de vulnérabilités complet sur une machine cible Metasploitable 2.

Ce projet démontre ma capacité à :
- Configurer un outil de gestion des vulnérabilités (Nessus)
- Identifier, analyser et prioriser des failles de sécurité
- Interpréter les résultats et proposer des mesures correctives
- Travailler dans un environnement virtualisé et isolé

## 🧰 Environnement utilisé

| Composant | Détails |
|----------|---------|
| Machine d’analyse | Kali Linux (VM) |
| Outil de scan | Nessus Essentials |
| Machine cible | Metasploitable 2 |
| Hyperviseur | VirtualBox |
| Réseau | NAT ou Host‑Only |

## 🚀 Étapes réalisées

### 1. Installation et configuration de Nessus
- Téléchargement de Nessus Essentials depuis Tenable
- Installation sur Kali Linux
- Activation via clé d’enregistrement
- Mise à jour des plugins
- Accès à l’interface Web (port 8834)
  
   <img width="640" height="507" alt="image" src="https://github.com/user-attachments/assets/e1da9d06-37ac-4a3c-8389-d26e90dcfe61" />

  <img width="1092" height="806" alt="image" src="https://github.com/user-attachments/assets/dc47a5da-f469-4c6f-885f-97bc93ee6afd" />


### 2. Préparation de l’environnement
- Démarrage de Metasploitable 2
- Vérification de la connectivité réseau (ping, nmap)
- Identification de l’adresse IP cible

  <img width="898" height="606" alt="image" src="https://github.com/user-attachments/assets/0d02adba-603a-4b4a-afa5-388d1ad4b18e" />


### 3. Création et lancement du scan
- Création d’un Basic Network Scan
- Définition de la cible : IP de Metasploitable 2
- Paramétrage des options
- Lancement du scan

  <img width="717" height="532" alt="image" src="https://github.com/user-attachments/assets/35772547-f692-46fe-8ca2-e9923fcc9301" />

  <img width="1087" height="797" alt="image" src="https://github.com/user-attachments/assets/d840921d-d104-4438-ac15-731a4db27cc9" />


### 4. Résultats 
- Nombre total de vulnérabilités détectées : 68
- Critiques : 10
- Élevées : 6
- Moyennes : 24
- Faibles : 9
  <img width="1087" height="666" alt="image" src="https://github.com/user-attachments/assets/854a605c-0938-4413-9b10-4942770786c1" />

  <img width="950" height="526" alt="image" src="https://github.com/user-attachments/assets/36d379f0-1bf7-4126-afd8-1c7aef048a81" />


  ### 5. Analyse des résultats
Nessus a détecté plusieurs vulnérabilités critiques, notamment :
- VNC avec mot de passe faible
- Backdoors actives
- Protocoles SSL obsolètes
- Services non sécurisés comme Telnet et rlogin
  
  <img width="1090" height="797" alt="image" src="https://github.com/user-attachments/assets/cf0548c1-b6dc-4c21-8ce4-0f036ac67a12" />

Ces vulnérabilités peuvent permettre à un attaquant de :
- Obtenir un accès shell
- Voler des données
- Contrôler le système


### 6. Recommandations proposées
- Changer les mots de passe faibles en forts
- Désactivation SSLv2 et SSLv3
- Supprimer les backdoor
- Désactivé Telnet et rlogin
- Mettre à jour le système

  <img width="942" height="550" alt="image" src="https://github.com/user-attachments/assets/970db020-be36-476b-9581-9140d392102d" />



## 📚 Compétences développées
- Gestion des vulnérabilités
- Analyse de rapports Nessus
- Interprétation des CVE
- Évaluation des risques
- Mise en place d’un environnement de test sécurisé
- Méthodologie SOC / Blue Team


