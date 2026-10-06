# Konfiguration

FraseKill kann auf zwei Arten konfiguriert werden: über das **visuelle Script-Einstellungen-Panel**, mit dem du die meisten Optionen aus `config.lua` und `config_server.lua` ohne Codeänderungen anpassen kannst, oder direkt in diesen Dateien.

Einige private Einstellungen wie Webhooks und sensible Optionen bleiben ausschließlich in den Ressourcendateien.

## Visuelles Konfigurationspanel

Das ist derselbe Panel-Typ wie in FraseKill Admin. Du kannst ihn hier ausprobieren, bevor du etwas auf deinem Server änderst.

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=de" %}

[**Konfigurationspanel im Vollbild öffnen →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=de)

{% hint style="info" %}
Die Demo verbindet sich nicht mit FiveM, SQL oder Tebex und verändert keinen Server.
{% endhint %}

## Über Dateien konfigurieren

- `config.lua` — Sprache, Aussehen, Befehle, Standardwerte, Animationen und visuelles Verhalten.
- `config_server.lua` — Zugriff, Administration, Tebex, Sicherheit und Serveroptionen.
- `server/webhooks.lua` — Discord-Webhooks.

{% hint style="info" %}
Wenn du wenig Erfahrung hast, nutze das **visuelle Panel** für normale Einstellungen und bearbeite Dateien nur wenn nötig.
{% endhint %}
