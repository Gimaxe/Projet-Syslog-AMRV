# Procédure d'installation RSyslog
## Prérequis
- ### Serveur Web (WordPress)
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
    ```bash
    cd /etc
    sudo cp rsyslog.conf rsyslog.conf.bak
    sudo vim rsyslog.conf
    ```


    ```conf
    #################
    #### MODULES ####
    #################

    module(load="imuxsock") # provides support for local system logging
    module(load="imklog")   # provides kernel logging support
    #module(load="immark")  # provides --MARK-- message capability
    ```
    *Ajouter ces lignes à la fin de la section **"MODULES"** du fichier rsyslog.conf*

    ```conf
    # provides UDP syslog reception
    module(load="imudp")
    input(type="imudp" port="514")
    # provides TCP syslog reception
    module(load="imtcp")
    input(type="imtcp" port="514")
    ```
