# Tebex et expirations

Activez `Config.Tebex.Enabled = true` dans `config_server.lua`, puis créez des plans en minutes, heures, jours, semaines, mois, années ou permanents.

Achat/renouvellement :
```text
frasekill_tebex {id} month {transaction}
```

Remboursement/chargeback d’une transaction précise :
```text
frasekill_tebex_revoke {id} {transaction}
```

Les renouvellements s’ajoutent au temps restant et chaque transaction est enregistrée séparément. Les plans temporaires expirent automatiquement. `Config.ExpiryNotifications` gère les alertes avant expiration.
