# Thim Core Advanced

Thim Core Advanced est un plugin serveur pour Nova-Life Amboise. Il regroupe les outils de gestion courante du serveur et ajoute des modules de surveillance, Modération, Optimisation, Administration, ect.. 

Le plugin fonctionne avec une clé de licence valide. Sans activation, les modules restent désactivés.

## Fonctionnalités principales

- Messages d'accueil et annonces automatiques.
- Rotations de messages.
- Gestion du cycle jour et nuit.
- Gestion de la météo.
- Redémarrages programmés.
- Mode maintenance.
- Nettoyage anti-lag.
- Événements, sondages et votes.
- Annonces d'entreprise.
- Statistiques et informations du serveur.
- Modération du chat et détection de mots configurés.
- Gestion de l'inactivité des joueurs.
- Limitation des connexions.
- Protection contre l'utilisation répétée des commandes.
- Journalisation vers Discord.

## Modules avancés

### Surveillance de l'argent

Le plugin compare l'évolution de la fortune des joueurs et signale les variations dépassant les seuils configurés. Une déconnexion automatique peut être activée. Le système détecte et signale les variations, mais ne modifie pas directement l'argent du joueur.

### Surveillance des inventaires

Les changements inhabituels dans les inventaires peuvent être enregistrés et signalés au staff selon les limites définies dans la configuration.

### Suivi de l'économie

Le plugin conserve des statistiques sur l'argent en circulation, permet d'identifier les personnages les plus fortunés et peut signaler une hausse anormale de l'économie globale.

### Temps de jeu

Le temps passé en jeu est enregistré par personnage. Une récompense de fidélité peut être configurée.

## Commandes principales

Le préfixe `core` est utilisé par défaut et peut être modifié dans la configuration.

| Commande | Fonction |
| --- | --- |
| `/core panel` | Ouvrir le panneau de gestion |
| `/core admin` | Ouvrir le panneau d'administration |
| `/core annonce <message>` | Diffuser une annonce |
| `/core clearlag` | Lancer un nettoyage immédiat |
| `/core restart [secondes] [raison]` | Programmer un redémarrage |
| `/core maintenance on\|off [raison]` | Gérer le mode maintenance |
| `/core stats` | Afficher les statistiques |
| `/core heure <0-23>` | Régler l'heure de référence |
| `/core meteo <type>` | Appliquer une météo |
| `/core reload` | Recharger la configuration |
| `/core aide` | Afficher l'aide des commandes |
| `/pub [message]` | Publier une annonce d'entreprise |
| `/sondage` | Créer et gérer un sondage |
| `/vote [numéro]` | Participer au sondage actif |
| `/event` | Créer et gérer un événement |
| `/uptime` | Afficher le temps de fonctionnement |
| `/serverinfo` | Afficher l'état du serveur |

## Gestion de la licence

Les commandes suivantes doivent être exécutées depuis la console du serveur :

```text
coreadv.license.add <cle>
coreadv.license.remove <cle>
coreadv.license.list
```

Une clé ne doit jamais être publiée dans un dépôt, une capture d'écran ou un rapport de problème.

## Installation

La procédure complète est disponible dans [INSTALLATION.md](INSTALLATION.md).

## Compatibilité

- Nova-Life
- Plugin serveur autonome
- Aucune dépendance externe requise

## Distribution

La version compilée est distribuée depuis les Releases du dépôt. Le code source et les clés de licence ne sont pas inclus.

## Crédits
Développé par Thimoute.
Proposé et mis en avant par CookYourServ.
Support : https://discord.gg/8DG7AsMDC
