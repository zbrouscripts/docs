# Instalacja

## Szybki start

1. Zainstaluj i uruchom `oxmysql`.
2. Dodaj `zbrou_frasekill` do serwera.
3. Sprawdź uprawnienia i konfigurację przed udostępnieniem serwera graczom.
4. Dodaj do `server.cfg`:

```cfg
ensure oxmysql
ensure zbrou_frasekill
```

5. Zrestartuj zasób lub serwer.

FraseKill automatycznie tworzy i migruje tabele, gdy `Config.Storage.AutoCreate = true`, co jest ustawieniem domyślnym. Możesz też wykonać ręcznie `sql/install.sql`.

## Pierwszy administrator

Uruchom:

```text
/frasekilladmin
```

Jeśli nie masz jeszcze uprawnień, menu pokaże dokładną linię ACE do skopiowania do `server.cfg`. Możesz też dodać ją ręcznie:

```cfg
add_ace identifier.license:TWOJA_LICENSE zbrou.frasekill.admin allow
```

Po zmianie uprawnień ACE zrestartuj zasób.

## Sprawdzenie

- `/frasekill` otwiera edytor, jeśli gracz ma dostęp.
- `/frasekilladmin` otwiera panel administracyjny.
- `/frasekillstatus` pokazuje diagnostykę administratorom.

`/frasekilltest` jest narzędziem deweloperskim i w publicznej wersji jest wyłączony.
