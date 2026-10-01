# Installation

## Démarrage rapide

1. Installez et démarrez `oxmysql`.
2. Ajoutez `zbrou_frasekill` à votre serveur.
3. Vérifiez les permissions et la configuration avant d’ouvrir le serveur au public.
4. Ajoutez dans `server.cfg` :

```cfg
ensure oxmysql
ensure zbrou_frasekill
```

5. Redémarrez la ressource ou le serveur.

FraseKill crée et migre automatiquement ses tables lorsque `Config.Storage.AutoCreate = true`, valeur par défaut. Pour une installation manuelle, vous pouvez aussi exécuter `sql/install.sql`.

## Premier administrateur

Exécutez :

```text
/frasekilladmin
```

Si vous n’avez pas encore la permission, le menu affiche la ligne ACE exacte à copier dans `server.cfg`. Vous pouvez aussi l’ajouter manuellement :

```cfg
add_ace identifier.license:VOTRE_LICENSE zbrou.frasekill.admin allow
```

Redémarrez la ressource après toute modification ACE.

## Vérification

- `/frasekill` ouvre l’éditeur si le joueur a accès.
- `/frasekilladmin` ouvre le panneau d’administration.
- `/frasekillstatus` affiche le diagnostic aux administrateurs.

`/frasekilltest` est réservé au développement et désactivé dans la version publique.
