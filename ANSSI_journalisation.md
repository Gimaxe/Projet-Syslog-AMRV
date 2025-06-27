# Liste point important obligatoire :
- crucial de disposer d’équipements synchronisés sur la même source de temps
    NTP (Network Time Protocol) est le protocole le plus fréquemment utilisé pour la synchronisation des horloges

- Il doit etre executable et la lecture possible pour un humain

- Utilisé des logs précise avec uniquement les information essentiel et gérer la verbosité est important pour perdre aucun log pour sucharge

- Prévoir de l'espace de stockage local et un script d'export des logs machines afin d'avoir une copie externe des logs ou system de centralisation des logs

- Armoniser les formats de log sans modifier les logs générer avant envoie

- transfert en temps différé (maximmum toutes les quelque heures et recommandé en temps réel)

- Mode pull (le serveur qui se connecte pour récupérer les logs sur les machines) 
Choix d'un mode pull ou push (pull compte unique avec authorisation spécial ou push mais plus risqué pour la connexion sur les serveur centraux)



# Liste point important non essentiel

vérifier régulièrement que tous les systèmes du SI sont bien journalisés

Un fichier de log doit etre demander dans un cahier des charges de projet informatique

il doit etre structuré afin de simplifier la lecture 

Il doit etre détaillé (posséder les information comme utilisateur,nom de machine, IP, action réaliser)

Il faut trier les log en catégorie évènements 

Il système de suppression automatique passé une certaine date doit etre mis en place

Activer la journalisation sur un grand nombre de matériels

Journaliser les empreintes des fichiers potentiellement malveillants

Le niveau de verbosité et de configuration des logs est important pour perdre aucun log pour sucharge

- redondance du système de centralisation de logs

les serveurs intermédiaires peuvent apporter des fonctionnalités additionnelles (compression de fichier, chiffrement)

