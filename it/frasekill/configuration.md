# Configurazione

FraseKill può essere configurato in due modi: dal **pannello visuale delle Impostazioni script**, che permette di cambiare la maggior parte delle opzioni di `config.lua` e `config_server.lua` senza modificare codice, oppure direttamente da quei file.

Alcune opzioni private, come webhook e impostazioni sensibili, restano solo nei file della risorsa.

## Pannello visuale di configurazione

È lo stesso tipo di pannello che trovi dentro FraseKill Admin. Puoi provarlo qui prima di modificare il server.

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=it" %}

[**Apri il pannello di configurazione a schermo intero →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=it)

{% hint style="info" %}
La demo non si collega a FiveM, SQL o Tebex e non modifica alcun server.
{% endhint %}

## Configurare dai file

- `config.lua` — lingua, aspetto, comandi, valori predefiniti, animazioni e comportamento visuale.
- `config_server.lua` — accesso, amministrazione, Tebex, sicurezza e opzioni server.
- `server/webhooks.lua` — webhook Discord.

{% hint style="info" %}
Se non hai molta esperienza, usa il **pannello visuale** per le impostazioni normali e modifica i file solo quando serve.
{% endhint %}
