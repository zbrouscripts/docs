# Installation

## Schnellstart

1. Installiere und starte `oxmysql`.
2. Füge `zbrou_frasekill` deinem Server hinzu.
3. Prüfe Berechtigungen und Konfiguration, bevor der Server öffentlich genutzt wird.
4. Ergänze in `server.cfg`:

```cfg
ensure oxmysql
ensure zbrou_frasekill
```

5. Starte die Ressource oder den Server neu.

FraseKill erstellt und migriert seine Tabellen automatisch, wenn `Config.Storage.AutoCreate = true` aktiviert ist. Das ist die Standardeinstellung. Alternativ kann `sql/install.sql` manuell ausgeführt werden.

## Erster Administrator

Führe aus:

```text
/frasekilladmin
```

Falls noch keine Berechtigung vorhanden ist, zeigt das Menü die genaue ACE-Zeile für `server.cfg`. Manuell sieht sie so aus:

```cfg
add_ace identifier.license:DEINE_LICENSE zbrou.frasekill.admin allow
```

Starte die Ressource nach Änderungen an ACE-Berechtigungen neu.

## Prüfung

- `/frasekill` öffnet den Editor, wenn der Spieler Zugriff hat.
- `/frasekilladmin` öffnet das Administrationspanel.
- `/frasekillstatus` zeigt Administratoren Diagnoseinformationen.

`/frasekilltest` ist nur für Entwicklung gedacht und in der öffentlichen Version deaktiviert.
