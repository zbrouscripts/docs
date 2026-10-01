# Tebex und Ablaufzeiten

Aktiviere `Config.Tebex.Enabled = true` in `config_server.lua` und definiere Pläne in Minuten, Stunden, Tagen, Wochen, Monaten, Jahren oder permanent.

Kauf/Verlängerung:
```text
frasekill_tebex {id} month {transaction}
```

Refund/Chargeback einer konkreten Transaktion:
```text
frasekill_tebex_revoke {id} {transaction}
```

Verlängerungen werden auf die Restzeit addiert und jede Transaktion wird separat gespeichert. Zeitpläne laufen automatisch ab. `Config.ExpiryNotifications` steuert Ablaufwarnungen.
