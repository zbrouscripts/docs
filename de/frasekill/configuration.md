# Konfiguration

FraseKill trennt die Einstellungen in eine gemeinsam genutzte Datei und eine reine Server-Datei.

## `config.lua`

Enthält visuelle und gemeinsam genutzte Optionen. **Keine Secrets, Tokens oder Webhooks hier eintragen.**

- `Config.Debug`: in Produktion `false` lassen.
- `Config.Command` / `AdminCommand`: Editor- und Admin-Befehl.
- `Config.Locale`: Standardsprache.
- `Config.MaxCharacters`: maximale Zeichenanzahl pro Phrase.
- `Config.DefaultSlotMode`: `fixed` nutzt den gewählten Slot; `random` wählt zufällig aus gültigen, für Random aktivierten Slots.
- `Config.Death.Adapter = 'auto'`: erkennt die verfügbare Integration automatisch. Alternativ können `esx_ambulancejob`, `qb-ambulancejob`, `qbx_medical` oder `standalone` erzwungen werden.

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

- `timed`: blendet nach `Seconds` aus, auch wenn der Spieler noch tot ist.
- `death_state`: bleibt während des Todes sichtbar und verschwindet beim Wiederbeleben. `FailsafeSeconds` verhindert ein dauerhaft festhängendes Overlay.
- `smart`: folgt dem Todesstatus, verwendet aber zusätzlich `MaxSeconds` als harte Obergrenze.

`MinVisibleMs` garantiert eine minimale Sichtbarkeit.

Außerdem enthält `config.lua` Standardwerte, Grenzen, Schriftarten, Animationen, Sprachen und Presets. `Config.Developer.Enabled` sollte in Produktion `false` bleiben.

## `config_server.lua`

Wird **nur serverseitig** ausgeführt.

- `Config.Storage`: Tabelle, Auto-Erstellung und Identifier (`license`, `character`, `custom`). `license` wird empfohlen.
- `Config.GroupAccess`: Jobs, GuilleGangs V2, QB/Qbox-Gangs und Custom-Gruppen; mehrere Systeme können gleichzeitig aktiv sein.
- Gruppen werden intern getrennt (`job:police`, `guille:ballas`, `frameworkgang:vagos`), damit gleiche Namen nicht kollidieren. Mindestgrad z. B. `job:police@2`.
- `Config.Access.Mode`: `everyone`, `managed`, `ace` oder `custom`; `managed` ist für VIP/Bezahlzugang empfohlen.
- `Config.Admin`: ACE und Owners des Admin-Panels.
- `Config.KillerName`: FiveM-Name, Charaktername oder Custom-Resolver.
- `Config.Moderation`: URL-/Wortfilter und serverseitige Custom-Validierung.
- `Config.Security`: Cooldowns für Speichern, Reset und Admin-Aktionen.
- `Config.ExpiryNotifications`: Ablaufwarnungen.
- `Config.Logs`: aktiviert Logs; Webhooks gehören in `server/webhooks.lua`.
- `Config.Tebex`: zeitlich begrenzte oder permanente Pläne.
- `Config.Diagnostics`: Admin-Befehl `/frasekillstatus`.
