# Permessi e amministrazione

## Owner principale

L'owner ha accesso completo a FraseKill Admin.

Aggiungi una sola riga in `server.cfg`:

```cfg
add_ace identifier.license:TUA_LICENSE zbrou.frasekill.admin allow
```

Se non conosci la license, entra nel server e usa `/frasekilladmin`. FraseKill mostrerà la riga esatta da copiare.

## Aggiungere altri amministratori

Non servono altri ACE.

L'owner crea gli admin dal pannello e sceglie cosa possono fare: vedere i giocatori, gestire gli accessi, modificare/ripristinare FraseKill, gestire le regole e cambiare le impostazioni dello script.

Essere admin non dà automaticamente accesso giocatore a FraseKill.

## Accesso giocatori

Può essere permanente o temporaneo. Puoi anche dare accesso a job o gruppi.

Per Tebex, vedi **Impostazioni script → Accesso e Tebex**.
