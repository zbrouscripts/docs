# Configuration

FraseKill peut être configuré depuis le **panneau visuel des Réglages du script** ou directement dans `config.lua` et `config_server.lua`.

## Panneau visuel de configuration

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=fr" %}

[**Voir le panneau de configuration en plein écran →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=fr)

Le panneau permet de modifier la plupart des réglages courants sans toucher au code. Les options privées restent dans les fichiers de la ressource.

## Fichiers de configuration

- `config.lua` — langue, apparence, commandes et valeurs par défaut.
- `config_server.lua` — accès, administration, Tebex, sécurité et options serveur.
- `server/webhooks.lua` — webhooks Discord.

## Permissions et administration

Ajoute l'owner principal dans `server.cfg` :

```cfg
add_ace identifier.license:VOTRE_LICENSE zbrou.frasekill.admin allow
```

Si tu ne connais pas ta license, utilise `/frasekilladmin`.

Les autres administrateurs sont créés depuis le panneau avec des permissions séparées. Être admin ne donne pas automatiquement l'accès joueur à FraseKill.
