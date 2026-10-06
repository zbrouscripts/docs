# Installazione

## Cosa serve

- Un server FiveM.
- La risorsa `oxmysql` sul server.
- ESX, QBCore e Qbox sono opzionali. FraseKill funziona anche senza framework.
- `zbrou_utils` non è necessario.

## Aggiungere FraseKill

1. Metti la cartella nelle risorse e mantieni il nome `zbrou_frasekill`.
2. In `server.cfg`, assicurati che `oxmysql` sia prima di FraseKill:

```cfg
ensure oxmysql
ensure zbrou_frasekill
```

3. La SQL necessaria viene preparata automaticamente al primo avvio. È incluso anche `sql/install.sql` per chi preferisce farlo manualmente.
4. Riavvia la risorsa o il server.

## Accesso owner

```cfg
add_ace identifier.license:TUA_LICENSE zbrou.frasekill.admin allow
```

`/frasekilladmin` può mostrarti la riga esatta da copiare se non hai ancora il permesso.

## Strumento di test

`/frasekilltest` è disattivato di default. In `config.lua`, cerca `Config.Developer` e imposta `Enabled = true`. Lascia `RequireAdmin = true`, poi rimetti `Enabled = false` quando hai finito.
