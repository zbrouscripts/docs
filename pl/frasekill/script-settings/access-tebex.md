# Dostęp i Tebex

Tryby:

- **Zarządzany dostęp**
- **Zarządzany dostęp + Tebex**
- **Własne sprawdzanie**

Dostęp może być stały lub czasowy.

Tebex jest opcjonalny.

```text
frasekill_tebex {id} month {transaction}
```

Dla zwrotu/chargebacku:

```text
frasekill_tebex_revoke {id} {transaction}
```

Dostępy czasowe wygasają automatycznie, a odnowienia dodają czas.
