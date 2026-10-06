# Installation

## Benötigt

- Einen FiveM-Server.
- Die Ressource `oxmysql` auf dem Server.
- ESX, QBCore und Qbox sind optional. FraseKill funktioniert auch ohne Framework.
- `zbrou_utils` wird nicht benötigt.

## FraseKill hinzufügen

1. Lege den Ordner in deine Ressourcen und behalte den Namen `zbrou_frasekill`.
2. Stelle in `server.cfg` sicher, dass `oxmysql` vor FraseKill steht:

```cfg
ensure oxmysql
ensure zbrou_frasekill
```

3. Die benötigte SQL wird beim ersten Start automatisch vorbereitet. `sql/install.sql` liegt zusätzlich für eine manuelle Einrichtung bei.
4. Starte die Ressource oder den Server neu.

## Owner-Zugriff

```cfg
add_ace identifier.license:DEINE_LICENSE zbrou.frasekill.admin allow
```

`/frasekilladmin` zeigt dir auch die genaue Zeile an, wenn du noch keine Berechtigung hast.

## Testwerkzeug

`/frasekilltest` ist standardmäßig deaktiviert. Suche in `config.lua` nach `Config.Developer` und setze `Enabled = true`. Lass `RequireAdmin = true` und setze danach wieder `Enabled = false`.
