# Procédure d'installation RSyslog
## Prérequis
- ### Serveur Applicatif
  - rsyslog
  - Pare-Feu (ufw)
- ### Serveur Collecteur (Base de Données)
  - MariaDB
  - rsyslog
  - rsyslog-mysql
  - Pare-Feu (ufw)
## Installation Serveur Collecteur 
 - ### MariaDB
   - #### Installation :
    ``` bash
    sudo apt install mariadb-server # Installation de la DB
    ```
- ### Pare-Feu (ufw)
  - #### Installation :
  ``` bash
    sudo apt install ufw # Installation du pare-feu
  ```
  - #### Configuration :
  ``` bash
    sudo ufw allow ssh # Autorisation du SSH
    sudo ufw allow 514 # Autorisation du Port 514
    sudo ufw enable # Activation du Pare-Feu
    sudo ufw status verbose # Affiche les règles du Pare-Feu
  ```
- ### rsyslog-mysql
    - #### Installation :
    ```bash
    sudo apt install rsyslog-mysql #Installation du plugin pour MariaDB
    ```
    - #### Configuration :
    ```yaml
