# Accesso e Tebex

Modalità disponibili:

- **Accesso gestito**
- **Accesso gestito + Tebex**
- **Controllo personalizzato**

Gli accessi possono essere permanenti o temporanei.

Tebex è opzionale.

```text
frasekill_tebex {id} month {transaction}
```

Per rimborso/chargeback:

```text
frasekill_tebex_revoke {id} {transaction}
```

Gli accessi temporanei scadono automaticamente e i rinnovi aggiungono tempo.
