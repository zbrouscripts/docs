# Configuration

FraseKill separates configuration into two files so it is clear which options are shared with clients and which must remain server-only.

## `config.lua`

This file contains shared and visual options. **Never put secrets, tokens or webhooks here.**

### General

```lua
Config.Debug = false
Config.Command = 'frasekill'
Config.AdminCommand = 'frasekilladmin'
Config.Locale = 'en'
Config.MaxCharacters = 70
```

- `Debug`: keep it `false` in production.
- `Command`: editor command.
- `AdminCommand`: admin-panel command.
- `Locale`: initial language.
- `MaxCharacters`: maximum length of each phrase.

### Slots

```lua
Config.DefaultSlotMode = 'fixed' -- fixed | random
```

- `fixed`: uses the selected slot.
- `random`: randomly chooses from valid slots enabled for random mode.

### Death detection

```lua
Config.Death.Adapter = 'auto'
```

`auto` tries to detect the available integration automatically. You can also force `esx_ambulancejob`, `qb-ambulancejob`, `qbx_medical` or `standalone`.

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

- `timed`: hides after `Seconds`, even if the player is still dead.
- `death_state`: stays visible while the player is dead and hides on revive. `FailsafeSeconds` prevents a stuck overlay if another resource fails to report the revive.
- `smart`: follows the death state but also applies `MaxSeconds` as a hard maximum.

`MinVisibleMs` prevents the phrase from disappearing so quickly that it cannot be read.

### Customization

`config.lua` also contains default values, size/position/speed ranges, fonts, animations, languages and default presets.

### Test tool

```lua
Config.Developer.Enabled = false
```

Keep it disabled in production. If you enable it on a test server, keep `RequireAce = true`.

---

## `config_server.lua`

This file runs **only on the server**. It contains permissions, access rules, jobs/groups, Tebex and logic that should never be sent to clients.

### Database and storage

```lua
Config.Storage.Identifier = 'license'
```

- `license`: one profile per Rockstar license. Recommended.
- `character`: one profile per framework character when supported.
- `custom`: uses `CustomIdentifier` to return your own stable identifier.

`AutoCreate = true` creates and migrates tables automatically.

### Jobs, gangs and groups

`Config.GroupAccess` can enable several systems at the same time: Jobs, GuilleGangs V2, native QB/Qbox gangs or a custom resolver.

Permissions are namespaced internally so equal names from different systems never collide:

```text
job:police
guille:ballas
frameworkgang:vagos
custom:vip
```

A minimum grade can also be required, for example `job:police@2`.

### Access mode

```lua
Config.Access.Mode = 'managed'
```

- `everyone`: everyone can use FraseKill.
- `managed`: admin panel + groups + ACE + Tebex. Recommended for monetized access.
- `ace`: only the configured ACE permission.
- `custom`: access is decided by `CustomCheck`.

### Administration

`Config.Admin.AcePermission` defines the admin ACE. `Owners` can contain identifiers directly, although ACE is recommended.

### Killer name

`Config.KillerName.Mode` supports `game`, `character` and `custom`.

### Moderation

`Config.Moderation` can block URLs, blocked words and run a custom server-side validator.

### Security

`Config.Security` controls save, reset and admin-action cooldowns. Avoid setting them to `0` on public servers.

### Expirations

`Config.ExpiryNotifications` controls how often temporary access is checked and when warnings are sent.

### Logs

Enable logs with `Config.Logs.Enabled`. Webhook URLs belong only in `server/webhooks.lua`.

### Tebex

`Config.Tebex` defines minute, hour, day, week, month, year or permanent plans. See **Tebex and expirations** for the full setup.

### Diagnostics

`Config.Diagnostics` controls `/frasekillstatus`, an admin-only command for database, detection and integration diagnostics.
