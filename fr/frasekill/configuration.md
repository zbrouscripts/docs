# Configuration

FraseKill sépare les réglages entre un fichier partagé et un fichier réservé au serveur.

## `config.lua`

Il contient les options visuelles et partagées. **N’y placez jamais de secrets, tokens ou webhooks.**

- `Config.Debug` : laissez `false` en production.
- `Config.Command` / `AdminCommand` : commandes de l’éditeur et du panneau admin.
- `Config.Locale` : langue initiale.
- `Config.MaxCharacters` : longueur maximale de chaque phrase.
- `Config.DefaultSlotMode` : `fixed` utilise le slot sélectionné ; `random` choisit parmi les slots valides activés pour l’aléatoire.
- `Config.Death.Adapter = 'auto'` : détecte automatiquement l’intégration disponible. Vous pouvez aussi forcer `esx_ambulancejob`, `qb-ambulancejob`, `qbx_medical` ou `standalone`.

### `Config.Display.Mode`

```lua
Config.Display = {
    Mode = 'death_state', -- timed | death_state | smart
    Seconds = 10,
    MaxSeconds = 20,
    FailsafeSeconds = 120,
    MinVisibleMs = 850
}
```

- `timed` : masque FraseKill après `Seconds`, même si le joueur est encore mort.
- `death_state` : reste affiché pendant la mort et disparaît à la réanimation. `FailsafeSeconds` évite un overlay bloqué.
- `smart` : suit l’état de mort mais ajoute `MaxSeconds` comme limite absolue.

`MinVisibleMs` garantit un temps d’affichage minimum.

Ce fichier contient aussi les valeurs visuelles, limites, polices, animations, langues et presets initiaux. Gardez `Config.Developer.Enabled = false` en production.

## `config_server.lua`

Ce fichier s’exécute **uniquement côté serveur**.

- `Config.Storage` : table, création automatique et identifiant (`license`, `character`, `custom`). `license` est recommandé.
- `Config.GroupAccess` : Jobs, GuilleGangs V2, gangs QB/Qbox et groupes personnalisés, activables ensemble.
- Les groupes sont namespacés (`job:police`, `guille:ballas`, `frameworkgang:vagos`) pour éviter les collisions. Un grade minimum est possible avec `job:police@2`.
- `Config.Access.Mode` : `everyone`, `managed`, `ace` ou `custom`. `managed` est recommandé pour un accès VIP/payant.
- `Config.Admin` : ACE et owners du panneau admin.
- `Config.KillerName` : nom FiveM, nom du personnage ou resolver custom.
- `Config.Moderation` : URLs, mots bloqués et validation custom côté serveur.
- `Config.Security` : cooldowns de sauvegarde/reset/actions admin.
- `Config.ExpiryNotifications` : alertes avant expiration.
- `Config.Logs` : active les logs ; les URLs restent dans `server/webhooks.lua`.
- `Config.Tebex` : plans temporaires ou permanents.
- `Config.Diagnostics` : commande admin `/frasekillstatus`.
