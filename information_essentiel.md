# Contexte (analyse de l'existant)

L'application actuelle est un site web créé et géré avec nginx.  \
Les journaux (logs) sont générés et stockés localement sur le serveur web. \
Aucune gestion n'est faites sur les logs

# Expression du besoin

Afin de se conformer aux recommandations de l’ANSSI, il est nécessaire de mettre en place une seconde machine dédiée à la journalisation centralisée.  
Cette machine devra permettre :

- la sauvegarde des logs ;
- l’affichage centralisé des journaux collectés.

# Objectif du projet

- Collecter les logs, les centraliser et les stocker sur un serveur distant.  
- Fournir un affichage graphique de l’ensemble des journaux collectés.

# Fonctions principales

- Copie des journaux de l’ensemble de l’infrastructure vers le serveur de collecte.  
- Affichage des journaux sur le serveur de collecte.  
- Sauvegarde automatique des logs sur le serveur de collecte.

# Critères de performance

- Actualisation manuellement de la page .  
- Récupération des journaux automatique via rsyslog.

# Contraintes techniques

- Respect des recommandation de ANSSI
- Utilisation de **rsyslog**.  
- Deux machines minimum requises.
