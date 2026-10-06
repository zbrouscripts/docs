# Configuration

FraseKill peut être configuré de deux façons :

- **Panneau d'administration** — la solution la plus simple.
- **Fichiers de configuration** — si tu préfères modifier les fichiers Lua.

Choisis le mode dans **FraseKill Admin → Réglages du script**.

Le panneau permet de modifier visuellement la langue, les couleurs, les valeurs par défaut, la détection de mort, les accès, Tebex, les règles et les notifications. Chaque option possède un `?` avec une explication simple.

## Tester le panneau avant de configurer

Ouvre une **démo interactive des Réglages du script** avec le même style visuel que le vrai panneau. Tu peux tester Classic/Liquid Glass, les couleurs, switches, menus, le verrouillage par fichiers et la restauration des valeurs.

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=fr" %}

[**Ouvrir la démo en plein écran →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=fr)

{% hint style="info" %}
Cette démo ne se connecte pas à FiveM, SQL ou Tebex et ne modifie aucun serveur.
{% endhint %}

- `config.lua` — apparence, langue, commandes, valeurs par défaut et animations.
- `config_server.lua` — accès, administration, Tebex, sécurité et réglages serveur.
- `server/webhooks.lua` — webhooks Discord.
