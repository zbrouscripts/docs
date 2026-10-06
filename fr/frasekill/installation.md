# Installation

## Ce qu'il faut

- Un serveur FiveM.
- La ressource `oxmysql` sur le serveur.
- ESX, QBCore et Qbox sont optionnels. FraseKill fonctionne aussi sans framework.
- `zbrou_utils` n'est pas nécessaire.

## Ajouter FraseKill

1. Place le dossier dans tes ressources et garde le nom `zbrou_frasekill`.
2. Dans `server.cfg`, vérifie que `oxmysql` est avant FraseKill :

```cfg
ensure oxmysql
ensure zbrou_frasekill
```

3. La SQL nécessaire est préparée automatiquement au premier démarrage. Le fichier `sql/install.sql` est également inclus pour une installation manuelle.
4. Redémarre la ressource ou le serveur.

## Accès owner

```cfg
add_ace identifier.license:VOTRE_LICENSE zbrou.frasekill.admin allow
```

`/frasekilladmin` peut aussi afficher la ligne exacte à copier si tu n'as pas encore la permission.

## Outil de test

`/frasekilltest` est désactivé par défaut. Dans `config.lua`, cherche `Config.Developer` et mets `Enabled = true`. Garde `RequireAdmin = true`, puis remets `Enabled = false` quand tu as terminé.
