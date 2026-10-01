# Permissions et administration

Utilisez `/frasekilladmin` pour ouvrir le panneau. La méthode recommandée est ACE :

```cfg
add_ace identifier.license:VOTRE_LICENSE zbrou.frasekill.admin allow
```

Sans permission, le menu affiche automatiquement la ligne ACE à copier. L’onglet **Accès** gère les droits permanents ou temporaires et les Jobs/groupes activés dans `Config.GroupAccess`. L’onglet **Phrases** permet de rechercher un joueur, ouvrir ses détails, modifier les presets, réinitialiser/supprimer sa configuration, gérer son accès, ajouter une note interne et envoyer un message s’il est connecté. Les actions importantes sont toujours revalidées côté serveur.
