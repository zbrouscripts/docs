# Konfiguracja

FraseKill rozdziela ustawienia na plik współdzielony z klientem oraz plik działający wyłącznie po stronie serwera.

## `config.lua`

Zawiera opcje wizualne i współdzielone. **Nie umieszczaj tutaj sekretów, tokenów ani webhooków.**

- `Config.Debug`: na produkcji pozostaw `false`.
- `Config.Command` / `AdminCommand`: komendy edytora i panelu admina.
- `Config.Locale`: język początkowy.
- `Config.MaxCharacters`: maksymalna długość frazy.
- `Config.DefaultSlotMode`: `fixed` używa wybranego slotu; `random` losuje spośród poprawnych slotów włączonych do trybu losowego.
- `Config.Death.Adapter = 'auto'`: automatycznie wykrywa dostępną integrację. Można też wymusić `esx_ambulancejob`, `qb-ambulancejob`, `qbx_medical` lub `standalone`.

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

- `timed`: ukrywa FraseKill po `Seconds`, nawet jeśli gracz nadal nie żyje.
- `death_state`: pozostaje widoczny podczas śmierci i znika po revive. `FailsafeSeconds` zapobiega zablokowaniu overlayu.
- `smart`: śledzi stan śmierci, ale dodatkowo używa `MaxSeconds` jako twardego limitu.

`MinVisibleMs` zapewnia minimalny czas widoczności.

W tym pliku znajdują się też domyślne wartości wyglądu, limity, czcionki, animacje, języki i presety. Na produkcji pozostaw `Config.Developer.Enabled = false`.

## `config_server.lua`

Ten plik działa **wyłącznie po stronie serwera**.

- `Config.Storage`: tabela, automatyczne tworzenie i identyfikator (`license`, `character`, `custom`). Zalecane jest `license`.
- `Config.GroupAccess`: Jobs, GuilleGangs V2, gangi QB/Qbox i grupy custom. Kilka systemów może działać jednocześnie.
- Grupy używają namespace (`job:police`, `guille:ballas`, `frameworkgang:vagos`), więc identyczne nazwy nie kolidują. Minimalny grade: `job:police@2`.
- `Config.Access.Mode`: `everyone`, `managed`, `ace` lub `custom`. Dla płatnego/VIP dostępu zalecane jest `managed`.
- `Config.Admin`: ACE i owners panelu administracyjnego.
- `Config.KillerName`: nazwa FiveM, nazwa postaci lub resolver custom.
- `Config.Moderation`: blokada URL, słów i własna walidacja po stronie serwera.
- `Config.Security`: cooldowny zapisu/resetu/akcji admina.
- `Config.ExpiryNotifications`: ostrzeżenia o wygaśnięciu.
- `Config.Logs`: włącza logi; webhooki są tylko w `server/webhooks.lua`.
- `Config.Tebex`: plany czasowe lub stałe.
- `Config.Diagnostics`: komenda admina `/frasekillstatus`.
