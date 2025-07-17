
# Liste des livrables du projet

| Livrable            | Description                                                                                 |
|---------------------|---------------------------------------------------------------------------------------------|
| WebServer-AMRV      | Serveur principal hébergeant Nginx et les applications web                                  |
| DB-AMRV             | Serveur de base de données dédié à la collecte des journaux via Rsyslog                                        |
| MariaDB             | Base de données pour le stockage des informations                                           |
| Nextcloud           | Application web installée sur le serveur WebServer-AMRV pour le partage et la synchronisation de fichiers  |
| Nginx               | Serveur web et reverse proxy           installé sur WebServer-AMRV et DB-AMRV                                                     |
| Logcatch            | Site web permettant visualiser les logs dans la base de données             |
| Scripts d’intégration| Scripts permettant à Rsyslog de récupérer les logs depuis Nextcloud et les transférer vers

