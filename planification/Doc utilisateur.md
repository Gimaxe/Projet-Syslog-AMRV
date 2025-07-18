# Documentation utilisateur — Système de gestion des logs

## 1. Présentation 

Ici le système permet de gérer les logs générés par un serveur web. Il couvre la collecte, la configuration, la réception et le stockage des logs. Il y'a plusieurs acteurs tant principales que secondaires, chacun ayant des actions spécifiques.



---

## 2. Acteurs du système

### a. Utilisateur
- Accède au site web.
**https://logcatch.daisuke39.fr/**:
![Se connecter](Images/Capture1.png)

- S’authentifier avec ses identifiants.

![login/mdp](Images/Capture0.png)

-Sélectionner son instance

![Instance](Images/Capture2.png)
### b. Administrateur
**S'authentifier confère utilisateur**
- Configure les paramètres des logs.
![Filtres](Images/Capture4.png)

- Surveiller le fonctionnement du serveur.
![logs](Images/Capture5.png)
### c. Application
- Envoie des requêtes au serveur web.
![requêtes](Images/Capture10.png)
- Provoque la génération de logs.
![logs serveur](Images/Capture7.png)
### d. Serveur de collecte de logs
- Reçoit les logs envoyés par le serveur web.
- Lit et stocke les logs.
![logs serveur](Images/Capture8.png)
---

## 4. Remarques générales

- Les utilisateurs sont les administrateurs il n'y a pas de notion proprement dit d'utilisateurs et il n' y a pas de droits spécifiques conférés aux administrateurs tous ont les mêmes droits.

- Les administrateurs créent des comptes à l'aide d'un script stocké  à la racine du code .

![scripts](Images/Capture9.png)

- Les logs sont générés et tranférés automatiquement.
