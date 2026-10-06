# Zugriff und Tebex

Verfügbare Modi:

- **Verwalteter Zugriff**
- **Verwalteter Zugriff + Tebex**
- **Eigene Prüfung**

Zugriffe können dauerhaft oder zeitlich begrenzt sein.

Tebex ist optional.

```text
frasekill_tebex {id} month {transaction}
```

Für Rückerstattung/Chargeback:

```text
frasekill_tebex_revoke {id} {transaction}
```

Zeitliche Zugriffe laufen automatisch ab; Verlängerungen fügen weitere Zeit hinzu.
