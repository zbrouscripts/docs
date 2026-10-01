# Configurazione

FraseKill separa le opzioni tra un file condiviso e un file esclusivamente server-side.

## `config.lua`

Contiene impostazioni visive e condivise. **Non inserire segreti, token o webhook qui.**

- `Config.Debug`: lascia `false` in produzione.
- `Config.Command` / `AdminCommand`: comandi dell’editor e del pannello admin.
- `Config.Locale`: lingua iniziale.
- `Config.MaxCharacters`: numero massimo di caratteri per frase.
- `Config.DefaultSlotMode`: `fixed` usa lo slot selezionato; `random` sceglie tra gli slot validi abilitati al casuale.
- `Config.Death.Adapter = 'auto'`: rileva automaticamente l’integrazione disponibile. Puoi anche forzare `esx_ambulancejob`, `qb-ambulancejob`, `qbx_medical` o `standalone`.

### `Config.Display.Mode`

```lua
Config.Display = {
    Mode = 'death_state', -- timed | death_state | smart
    Seconds = 10,
    MaxSeconds = 20,
    FailsafeSeconds = 120,
    MinVisibleMs = 850
}
```

- `timed`: nasconde dopo `Seconds` anche se il giocatore è ancora morto.
- `death_state`: rimane visibile durante la morte e scompare al revive. `FailsafeSeconds` impedisce che l’overlay resti bloccato.
- `smart`: segue lo stato di morte ma applica anche `MaxSeconds` come limite massimo.

`MinVisibleMs` garantisce un tempo minimo di lettura.

Lo stesso file contiene valori visivi, limiti, font, animazioni, lingue e preset predefiniti. In produzione lascia `Config.Developer.Enabled = false`.

## `config_server.lua`

Viene eseguito **solo sul server**.

- `Config.Storage`: tabella, creazione automatica e identificatore (`license`, `character`, `custom`). `license` è consigliato.
- `Config.GroupAccess`: Jobs, GuilleGangs V2, gang QB/Qbox e gruppi custom; più sistemi possono essere attivi insieme.
- I gruppi sono separati con namespace (`job:police`, `guille:ballas`, `frameworkgang:vagos`) per evitare collisioni. Grado minimo: `job:police@2`.
- `Config.Access.Mode`: `everyone`, `managed`, `ace` o `custom`; `managed` è consigliato per accesso VIP/a pagamento.
- `Config.Admin`: ACE e owners del pannello admin.
- `Config.KillerName`: nome FiveM, nome personaggio o resolver custom.
- `Config.Moderation`: URL, parole bloccate e validatore custom server-side.
- `Config.Security`: cooldown di salvataggio/reset/admin.
- `Config.ExpiryNotifications`: avvisi di scadenza.
- `Config.Logs`: abilita i log; i webhook restano in `server/webhooks.lua`.
- `Config.Tebex`: piani temporanei o permanenti.
- `Config.Diagnostics`: comando admin `/frasekillstatus`.
