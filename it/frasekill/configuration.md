# Configurazione

FraseKill può essere configurato dal **pannello visuale delle Impostazioni script** oppure direttamente da `config.lua` e `config_server.lua`.

## Pannello visuale di configurazione

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=it" %}

[**Apri il pannello di configurazione a schermo intero →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=it)

Il pannello copre la maggior parte delle impostazioni normali senza modificare codice. Le opzioni private restano nei file della risorsa.

## File di configurazione

- `config.lua` — lingua, aspetto, comandi e valori predefiniti.
- `config_server.lua` — accesso, amministrazione, Tebex, sicurezza e opzioni server.
- `server/webhooks.lua` — webhook Discord.

## Permessi e amministrazione

Aggiungi l'owner principale in `server.cfg`:

```cfg
add_ace identifier.license:TUA_LICENSE zbrou.frasekill.admin allow
```

Se non conosci la license, usa `/frasekilladmin`.

Gli altri amministratori vengono creati dal pannello con permessi separati. Essere admin non concede automaticamente l'accesso giocatore a FraseKill.
