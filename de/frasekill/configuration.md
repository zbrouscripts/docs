# Konfiguration

FraseKill kann auf zwei Arten eingestellt werden:

- **Adminpanel** — die einfachere Variante.
- **Konfigurationsdateien** — wenn du lieber Lua-Dateien bearbeitest.

Wähle den Modus unter **FraseKill Admin → Script-Einstellungen**.

Im Panel kannst du Sprache, Farben, Standardwerte, Todeserkennung, Zugriff, Tebex, Regeln und Benachrichtigungen ändern. Jede Option besitzt ein `?` mit einer einfachen Erklärung.

## Panel vor der Konfiguration testen

Öffne eine **interaktive Demo der Script-Einstellungen** im gleichen visuellen Stil wie das echte Panel. Teste Classic/Liquid Glass, Farben, Schalter, Auswahlfelder, Datei-Sperrmodus und Zurücksetzen.

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=de" %}

[**Demo im Vollbild öffnen →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=de)

{% hint style="info" %}
Die Demo verbindet sich nicht mit FiveM, SQL oder Tebex und verändert keinen Server.
{% endhint %}

- `config.lua` — Aussehen, Sprache, Befehle, Standardwerte und Animationen.
- `config_server.lua` — Zugriff, Administration, Tebex, Sicherheit und Serveroptionen.
- `server/webhooks.lua` — Discord-Webhooks.
