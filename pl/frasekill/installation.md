# Instalacja

## Wymagania

- Serwer FiveM.
- Zasób `oxmysql` na serwerze.
- ESX, QBCore i Qbox są opcjonalne. FraseKill działa też bez frameworka.
- `zbrou_utils` nie jest wymagany.

## Dodanie FraseKill

1. Umieść folder w resources i pozostaw nazwę `zbrou_frasekill`.
2. W `server.cfg` upewnij się, że `oxmysql` jest przed FraseKill:

```cfg
ensure oxmysql
ensure zbrou_frasekill
```

3. Potrzebna SQL przygotowuje się automatycznie przy pierwszym uruchomieniu. Plik `sql/install.sql` jest również dołączony dla instalacji ręcznej.
4. Zrestartuj zasób lub serwer.

## Dostęp ownera

```cfg
add_ace identifier.license:TWOJA_LICENSE zbrou.frasekill.admin allow
```

`/frasekilladmin` może pokazać dokładną linię do skopiowania, jeśli nie masz jeszcze uprawnień.

## Narzędzie testowe

`/frasekilltest` jest domyślnie wyłączone. W `config.lua` znajdź `Config.Developer` i ustaw `Enabled = true`. Zostaw `RequireAdmin = true`, a po konfiguracji wróć do `Enabled = false`.
