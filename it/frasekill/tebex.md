# Tebex e scadenze

Abilita `Config.Tebex.Enabled = true` in `config_server.lua` e crea piani in minuti, ore, giorni, settimane, mesi, anni o permanenti.

Acquisto/rinnovo:
```text
frasekill_tebex {id} month {transaction}
```

Rimborso/chargeback di una transazione specifica:
```text
frasekill_tebex_revoke {id} {transaction}
```

I rinnovi si sommano al tempo residuo e ogni transazione viene registrata separatamente. I piani temporanei scadono automaticamente. `Config.ExpiryNotifications` gestisce gli avvisi.
