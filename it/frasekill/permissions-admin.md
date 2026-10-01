# Permessi e amministrazione

Apri il pannello con `/frasekilladmin`. Il metodo consigliato è ACE:

```cfg
add_ace identifier.license:TUA_LICENSE zbrou.frasekill.admin allow
```

Se non hai il permesso, FraseKill mostra automaticamente la riga ACE pronta da copiare. In **Accessi** puoi gestire permessi permanenti o temporanei e i Job/gruppi abilitati in `Config.GroupAccess`. In **Frasi** puoi cercare utenti, aprire i dettagli, modificare preset, resettare/eliminare configurazioni, dare o togliere accesso, salvare note interne e inviare messaggi ai giocatori online. Le azioni importanti vengono sempre riconvalidate server-side.
