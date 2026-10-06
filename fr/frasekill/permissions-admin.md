# Permissions et administration

## Owner principal

L'owner possède l'accès complet à FraseKill Admin.

Ajoute une seule ligne dans `server.cfg` :

```cfg
add_ace identifier.license:VOTRE_LICENSE zbrou.frasekill.admin allow
```

Si tu ne connais pas ta license, utilise `/frasekilladmin` dans le serveur. FraseKill affichera la ligne exacte à copier.

## Ajouter des administrateurs

Pas besoin d'ajouter d'autres ACE.

L'owner crée les administrateurs depuis le panneau et choisit leurs permissions : voir les joueurs, gérer les accès, modifier/réinitialiser FraseKill, gérer les règles et modifier les réglages du script.

Être administrateur ne donne pas automatiquement l'accès joueur à FraseKill.

## Accès joueur

L'accès peut être permanent ou limité dans le temps. Tu peux aussi donner l'accès à des jobs ou groupes.

Pour Tebex, voir **Réglages du script → Accès et Tebex**.
