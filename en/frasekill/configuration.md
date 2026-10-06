# Configuration

FraseKill has two configuration files and an optional visual **Script settings** panel.

## `config.lua`

Shared, non-secret settings: commands, default language, menu appearance, phrase defaults, fonts, animations, display behaviour and medical detection. Never place private tokens or webhooks here.

Important defaults:

```lua
Config.Locale = 'en'
Config.UI.Theme = 'classic'
Config.UI.AccentColor = '#0e58d8'
Config.UI.BackgroundColor = '#15181e'
Config.UI.BaseColor = '#1a1e25'
Config.DefaultSlotMode = 'fixed'
Config.MaxCharacters = 70
Config.Death.Adapter = 'auto'
```

`fixed` keeps the selected slot. `random` rotates between enabled valid slots so different kills can show different phrases.

## `config_server.lua`

Private/server-only settings: SQL/storage, jobs/groups, access mode, owner ACE, admin-role storage, killer-name resolvers, moderation, security, Tebex, logs, diagnostics and private callbacks.

Never move secrets from this file into client-visible files. Discord webhook URLs belong in `server/webhooks.lua`.

## Configuration source

The owner can choose **Configuration files** or **Administration panel** in Script settings.

- **Configuration files**: `config.lua` / `config_server.lua` are authoritative. Panel controls are locked. Saved panel values are kept only as a draft.
- **Administration panel**: supported safe options are loaded from the saved panel overrides.

Callbacks, secrets, webhook URLs and other advanced/private settings stay in files even when panel mode is enabled.
