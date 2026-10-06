# Script settings

Open **FraseKill Admin → Script settings** to change common resource options without editing Lua. The panel is made for server owners: every setting has a `?` tooltip with a plain-language explanation.

## Configuration mode

At the top, choose how you want to configure FraseKill:

- **Configuration files** — FraseKill uses `config.lua` and `config_server.lua`. The rest of the panel is locked and dimmed so it is obvious that it cannot be edited there.
- **Administration panel** — supported settings can be changed and saved directly from the interface.

Only the main owner can switch this mode. Switching modes does not delete player phrases or access grants.

## What you can change from the panel

### Interface

Default language, Classic/Liquid Glass theme, main commands and the three global menu colours.

- **Detail colour** — active buttons, switches, selected slot and highlights.
- **Background colour** — main menu background.
- **Base colour** — cards, fields, inactive slots and inner blocks.

All three colours have an individual reset icon that returns to the value defined in the configuration files.

### FraseKill

Character limit and the defaults used by new configurations: slot mode, phrase, enabled state, colours, size, glow, animations and killer-name appearance.

**Fixed** keeps the selected slot. **Random** rotates through your valid slots so different kills can show different phrases.

### Death detection

Medical adapter, the stage that counts as a valid death, how FraseKill is displayed and the maximum display time. If you use a supported ambulance resource, **Auto** is normally the best adapter option.

### Player access

Access mode, jobs/groups and expiry notifications. Available modes are **Managed access**, **Managed access + Tebex** and **Custom check**.

### Rules

Rule visibility and basic moderation filters. Rules and blocked words are managed from their own admin sections and validated on the server.

### Notifications

Enable or disable logs and choose the name used in Discord notifications. Webhook URLs remain in private server files only.

## Restore defaults

The global **Restore defaults** button is owner-only. It asks for confirmation, clears every saved override in **Script settings**, and returns the options to their original `config.lua` and `config_server.lua` values.

It does not delete:

- player phrases or presets;
- access grants or expiry dates;
- rules or blocked words;
- delegated administrators.

It also keeps the current configuration mode. Changes that need a resource restart remain marked as pending.

{% hint style="info" %}
Secrets, webhook URLs and Lua callbacks are never exposed in the web panel. Configure them only in private server files.
{% endhint %}
