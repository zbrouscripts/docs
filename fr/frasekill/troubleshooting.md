# Dépannage

## `/frasekill` ne s'ouvre pas

- Vérifie que le joueur a accès.
- En admin, utilise `/frasekillstatus`.
- Vérifie F8 et la console serveur.

## FraseKill Admin ne s'ouvre pas

Utilise `/frasekilladmin`. Si tu n'es pas encore owner, le script affiche la ligne à ajouter dans `server.cfg`.

## Réglages du script verrouillés

**Fichiers de configuration** est sélectionné. Choisis **Panneau d'administration** pour modifier depuis l'interface.

## Mauvais ambulance job

Ouvre **Réglages du script → Détection de mort**. Essaie d'abord **Auto**, puis choisis ton medical manuellement si nécessaire.

## Problème SQL

FraseKill prépare automatiquement ses tables. Pour une installation manuelle, utilise `sql/install.sql`.

## Tebex ne donne pas accès

Vérifie que **Accès géré + Tebex** est sélectionné et que le nom du plan correspond.

## Revenir aux valeurs d'origine

Utilise **Restaurer les valeurs par défaut**. Les phrases, accès, règles et administrateurs ne sont pas supprimés.
