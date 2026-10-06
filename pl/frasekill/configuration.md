# Konfiguracja

FraseKill można skonfigurować przez **wizualny panel Ustawień skryptu** albo bezpośrednio w `config.lua` i `config_server.lua`.

## Wizualny panel konfiguracji

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=pl" %}

[**Otwórz panel konfiguracji na pełnym ekranie →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=pl)

Panel obejmuje większość zwykłych ustawień bez edycji kodu. Prywatne opcje pozostają w plikach zasobu.

## Pliki konfiguracyjne

- `config.lua` — język, wygląd, komendy i wartości domyślne.
- `config_server.lua` — dostęp, administracja, Tebex, bezpieczeństwo i opcje serwera.
- `server/webhooks.lua` — webhooki Discord.

## Uprawnienia i administracja

Dodaj głównego ownera w `server.cfg`:

```cfg
add_ace identifier.license:TWOJA_LICENSE zbrou.frasekill.admin allow
```

Jeśli nie znasz swojej license, użyj `/frasekilladmin`.

Pozostali administratorzy są tworzeni w panelu z oddzielnymi uprawnieniami. Status admina nie daje automatycznie dostępu gracza do FraseKill.
