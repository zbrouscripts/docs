# Installazione

## Avvio rapido

1. Installa e avvia `oxmysql`.
2. Aggiungi `zbrou_frasekill` al server.
3. Controlla permessi e configurazione prima di aprire il server al pubblico.
4. Aggiungi a `server.cfg`:

```cfg
ensure oxmysql
ensure zbrou_frasekill
```

5. Riavvia la risorsa o il server.

FraseKill crea e migra automaticamente le tabelle quando `Config.Storage.AutoCreate = true`, valore predefinito. Se preferisci un’installazione manuale del database puoi eseguire anche `sql/install.sql`.

## Primo amministratore

Esegui:

```text
/frasekilladmin
```

Se non hai ancora i permessi, il menu mostra la riga ACE esatta da copiare in `server.cfg`. Puoi anche aggiungerla manualmente:

```cfg
add_ace identifier.license:TUA_LICENSE zbrou.frasekill.admin allow
```

Riavvia la risorsa dopo aver modificato i permessi ACE.

## Verifica

- `/frasekill` apre l’editor quando il giocatore ha accesso.
- `/frasekilladmin` apre il pannello di amministrazione.
- `/frasekillstatus` mostra la diagnostica agli amministratori.

`/frasekilltest` è solo per sviluppo ed è disattivato nella release pubblica.
