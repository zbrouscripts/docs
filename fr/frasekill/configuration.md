# Configuration

FraseKill peut être configuré de deux façons : depuis le **panneau visuel des Réglages du script**, qui permet de modifier la plupart des options de `config.lua` et `config_server.lua` sans toucher au code, ou directement dans ces fichiers.

Certaines options privées, comme les webhooks et les réglages sensibles, restent uniquement dans les fichiers de la ressource.

## Panneau visuel de configuration

C'est le même type de panneau que celui disponible dans FraseKill Admin. Tu peux le tester ici avant de modifier ton serveur.

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=fr" %}

[**Voir le panneau de configuration en plein écran →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=fr)

{% hint style="info" %}
La démo ne se connecte pas à FiveM, SQL ou Tebex et ne modifie aucun serveur.
{% endhint %}

## Configuration par fichiers

- `config.lua` — langue, apparence, commandes, valeurs par défaut, animations et comportement visuel.
- `config_server.lua` — accès, administration, Tebex, sécurité et options serveur.
- `server/webhooks.lua` — webhooks Discord.

{% hint style="info" %}
Si tu débutes, utilise le **panneau visuel** pour les réglages classiques et modifie les fichiers seulement si nécessaire.
{% endhint %}
