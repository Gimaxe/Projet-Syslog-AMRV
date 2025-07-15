# A faire
- Tous les équipements doivent être synchronisés sur la même horloge (NTP recommandé).
- Les logs doivent être lisibles par un humain.
- Transfert en temps réel recommandé, mais choix de récupération toutes les 5 min.
- Mode **pull** recommandé : le serveur vient chercher les logs. Plus sûr que le **push**.
- Préférer le transfert **TCP** pour la fiabilité. **UDP** possible, mais moins sûr (pertes).

# Optionnel
- Prévoir du stockage local + script d’export vers un système de centralisation.
- Utiliser des protocoles sécurisés pour les échanges (ex. : TLS).
- Définir une durée de rétention des logs (durée minimale et maximale de conservation des logs). \
  Mettre en place une suppression automatique des logs anciens.
- Restreindre l'accès aux fichiers de logs.
- Inclure des infos utiles : utilisateur, machine, IP, action.
- Maintenir les systèmes dans leur version la plus récente.
- Générer des alertes en cas d’erreur de récupération de logs.
- Mettre en place un système d’analyse de logs.

# Non nécessaire
- Harmoniser le format des logs sans altérer les originaux avant l'envoi.
- Utiliser des logs clairs, concis, sans information superflue. Bien gérer la verbosité.
- Vérifier régulièrement la journalisation de tous les systèmes du SI.
- Inclure les logs dans le cahier des charges d’un projet informatique.
- Gérer la bande passante (limitation, priorité des flux).
- Structurer les logs pour une lecture simple.
- Classer les logs par type d’événement.
- Activer la journalisation sur un maximum d’équipements.
- Journaliser les empreintes de fichiers suspects.
- Prévoir une redondance du système de centralisation.
- Utiliser des serveurs intermédiaires pour compression/chiffrement.
- Respecter le RGPD (données minimales, droits d’accès, etc...).