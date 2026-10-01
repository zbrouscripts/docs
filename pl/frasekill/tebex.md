# Tebex i wygasanie

W `config_server.lua` ustaw `Config.Tebex.Enabled = true` i utwórz plany w minutach, godzinach, dniach, tygodniach, miesiącach, latach lub stałe.

Zakup/odnowienie:
```text
frasekill_tebex {id} month {transaction}
```

Zwrot/chargeback konkretnej transakcji:
```text
frasekill_tebex_revoke {id} {transaction}
```

Odnowienia dodają czas do pozostałego okresu, a każda transakcja jest zapisywana osobno. Plany czasowe wygasają automatycznie. `Config.ExpiryNotifications` steruje ostrzeżeniami.
