# Configurazione

FraseKill può essere configurato in due modi:

- **Pannello di amministrazione** — la scelta più semplice.
- **File di configurazione** — se preferisci modificare i file Lua.

Scegli la modalità da **FraseKill Admin → Impostazioni script**.

Il pannello permette di cambiare lingua, colori, valori predefiniti, rilevamento morte, accesso, Tebex, regole e notifiche. Ogni opzione ha un `?` con una spiegazione semplice.

## Prova il pannello prima di configurarlo

Apri una **demo interattiva delle Impostazioni script** con lo stesso stile visivo del pannello reale. Puoi provare Classic/Liquid Glass, colori, switch, menu, blocco tramite file e ripristino.

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=it" %}

[**Apri la demo a schermo intero →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=it)

{% hint style="info" %}
È solo una demo della documentazione: non si collega a FiveM, SQL o Tebex.
{% endhint %}

- `config.lua` — aspetto, lingua, comandi, valori predefiniti e animazioni.
- `config_server.lua` — accesso, amministrazione, Tebex, sicurezza e opzioni server.
- `server/webhooks.lua` — webhook Discord.
