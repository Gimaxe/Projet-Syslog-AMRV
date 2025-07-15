# ✅ Points importants obligatoires

- Tous les équipements doivent être synchronisés sur la même horloge (NTP recommandé).
- Les logs doivent être lisibles par un humain et le système doit être exécutable.
- Utiliser des logs clairs, concis, sans information superflue. Bien gérer la verbosité.
- Prévoir du stockage local + script d’export vers une copie externe ou système de centralisation.
- Harmoniser le format des logs sans altérer les originaux avant envoi.
- Transfert en temps réel recommandé, sinon toutes les quelques heures maximum.
- Mode **pull** recommandé : le serveur vient chercher les logs. Plus sûr que le **push**.
- Préférer le transfert **TCP** pour fiabilité. **UDP** possible mais moins sûr (pertes).
- Utiliser des protocoles sécurisés (ex. : TLS).
- Définir une durée de rétention des logs.

# ⚠️ Points importants non essentiels

- Vérifier régulièrement la journalisation de tous les systèmes du SI.
- Restreindre l'accès aux fichiers de logs.
- Inclure les logs dans le cahier des charges d’un projet informatique.
- Gérer la bande passante (limitation, priorité des flux).
- Structurer les logs pour une lecture simple.
- Inclure des infos utiles : utilisateur, machine, IP, action.
- Classer les logs par type d’événement.
- Mettre en place une suppression automatique des logs anciens.
- Activer la journalisation sur un maximum d’équipements.
- Maintenir les systèmes dans un état sécurisé.
- Journaliser les empreintes de fichiers suspects.
- Bien configurer la verbosité pour éviter les pertes.
- Prévoir une redondance du système de centralisation.
- Utiliser des serveurs intermédiaires pour compression/chiffrement.
- Sécuriser les serveurs de collecte.
- Générer des alertes en cas d’erreur de récupération de logs.
- Mettre en place un système d’analyse de logs.
- Respecter le RGPD (données minimales, droits d’accès, etc.).
