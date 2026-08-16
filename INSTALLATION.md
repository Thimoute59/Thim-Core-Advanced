# Installation de Thim Core Advanced

## Prérequis

- Un serveur Nova-Life Amboise fonctionnel.
- Un accès au dossier `Plugins` et à la console du serveur.
- Le fichier `ThimCoreAdvanced.dll` téléchargé depuis une Release officielle.
- Une clé de licence valide.

## Installation

1. Arrêtez le serveur.
2. Placez `ThimCoreAdvanced.dll` directement dans le dossier `Plugins`.
3. Redémarrez le serveur.

Au premier démarrage, le plugin crée automatiquement :

```text
Plugins/ThimCoreAdvanced/
```

## Activation

Depuis la console du serveur, exécutez :

```text
coreadv.license.add <votre-cle>
```

Remplacez `<votre-cle>` par la clé fournie, puis redémarrez le serveur.

Pour afficher les licences actives sous une forme masquée :

```text
coreadv.license.list
```

Pour retirer une clé :

```text
coreadv.license.remove <cle>
```

Ne communiquez jamais votre clé dans un message public, une capture d'écran ou un ticket non privé.

## Fichiers générés

Le dossier du plugin contient notamment :

```text
Plugins/ThimCoreAdvanced/ThimCoreAdvancedConfig.json
Plugins/ThimCoreAdvanced/ThimCoreAdvancedConfig.exemple.json
```

`ThimCoreAdvancedConfig.json` est la configuration utilisée par le plugin.

`ThimCoreAdvancedConfig.exemple.json` sert uniquement d'exemple et n'est pas chargé par le plugin.

Les fichiers de licence, les journaux et les données persistantes sont également conservés dans le dossier du plugin.

## Configuration

1. Ouvrez `ThimCoreAdvancedConfig.json`.
2. Activez uniquement les modules nécessaires.
3. Réglez les permissions, les seuils et les messages.
4. Enregistrez le fichier.
5. Exécutez `/core reload` en jeu.

Le panneau `/core panel` permet également de modifier les réglages disponibles en jeu.

## Mise à jour

1. Arrêtez le serveur.
2. Sauvegardez `Plugins/ThimCoreAdvanced/`.
3. Remplacez uniquement `ThimCoreAdvanced.dll`.
4. Redémarrez le serveur.
5. Consultez les notes de version avant de modifier la configuration.

Ne supprimez pas les fichiers de configuration, de licence ou de données pendant une mise à jour.

## Désinstallation

1. Arrêtez le serveur.
2. Retirez `ThimCoreAdvanced.dll` du dossier `Plugins`.
3. Conservez ou supprimez `Plugins/ThimCoreAdvanced/` selon que vous souhaitez garder les données.
4. Redémarrez le serveur.

## Problèmes courants

### Aucun module ne démarre

- Vérifiez que la licence a été ajoutée depuis la console.
- Exécutez `coreadv.license.list`.
- Redémarrez le serveur après l'activation.
- Consultez `ThimCoreAdvanced.log`.

### La configuration ne se charge pas

- Vérifiez la syntaxe de `ThimCoreAdvancedConfig.json`.
- Comparez le bloc concerné avec `ThimCoreAdvancedConfig.exemple.json`.
- Corrigez le fichier puis exécutez `/core reload`.

### Le panneau est inaccessible

- Vérifiez les permissions définies pour `/core panel` et `/core admin`.
- Vérifiez que le préfixe des commandes n'a pas été modifié.
- Consultez la console et le journal du plugin.

## Crédits

Développé par Thimoute.

Proposé et mis en avant par CookYourServ.

Support : https://discord.gg/8DG7AsMDC
