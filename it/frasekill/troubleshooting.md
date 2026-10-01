# Risoluzione dei problemi

## `/frasekill` non si apre

Controlla l’accesso effettivo del giocatore, esegui `/frasekillstatus` come admin e verifica F8 e la console server.

## Le tabelle non vengono create

Assicurati che `oxmysql` parta prima di `zbrou_frasekill`. Se la creazione automatica è disattivata, esegui `sql/install.sql`.

## Il pannello admin non si apre

Aggiungi il permesso ACE corretto a `server.cfg` e riavvia la risorsa.

## FraseKill non scompare al revive

Controlla `Config.Display.Mode`, l’adapter mostrato da `/frasekillstatus` e `FailsafeSeconds`.

## Tebex non concede accesso

Controlla `Config.Tebex.Enabled`, che il comando sia eseguito da console/Tebex e che la chiave del piano sia esatta.

## Aiuto

Apri **Supporto** per entrare nel Discord ufficiale.
