# Konfiguration

FraseKill kann über das **visuelle Script-Einstellungen-Panel** oder direkt in `config.lua` und `config_server.lua` konfiguriert werden.

## Visuelles Konfigurationspanel

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=de" %}

[**Konfigurationspanel im Vollbild öffnen →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=de)

Das Panel deckt die meisten normalen Einstellungen ab. Private Optionen bleiben in den Ressourcendateien.

## Konfigurationsdateien

- `config.lua` — Sprache, Aussehen, Befehle und Standardwerte.
- `config_server.lua` — Zugriff, Administration, Tebex, Sicherheit und Serveroptionen.
- `server/webhooks.lua` — Discord-Webhooks.

## Berechtigungen und Administration

Füge den Haupt-Owner in `server.cfg` hinzu:

```cfg
add_ace identifier.license:DEINE_LICENSE zbrou.frasekill.admin allow
```

Wenn du deine License nicht kennst, nutze `/frasekilladmin`.

Weitere Admins werden im Panel mit getrennten Berechtigungen erstellt. Admin-Rechte geben nicht automatisch Spielerzugriff auf FraseKill.
