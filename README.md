# Somfy_Home_ALARM_API
Utilisation des api myfox pour somfy home alarm


1) deplacer le dossier private dans le repertoire parent
2) appeler la page control.php avec l'argument action= armed, disarmed, partial, weekend, notif_off ou notif_on
ex: control.php?action=armed

Description des commandes:
- armed : activer l'alarme
- disarmed : desactiver l'alarme
- partial: mode nuit : 3 etapes: desactivation de la notification sonore de la sirene, activation du mode nuit, réactivation de la notification sonore (après le délais d'activation)
- weekend: mode nuit sans réactivation des notifications sonores (évite d'être reveillé par la notification)
- notif_off: desactivation des notifications sonores de la sirene
- notif_on: activation des notifications sonores de la sirene


Changelog:
- ajout de la génération automatique du token à l'aide du nom d'utilisateur et mot de passe du fichier config.ini
- si le token est juste expiré -> raffraichissement du token
- ajout mode weekend
