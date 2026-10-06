# Configuration

FraseKill can be configured in two ways:

- **From the administration panel**, which is the easiest option if you do not want to edit files.
- **From the configuration files**, if you prefer to keep everything in Lua.

Choose the mode from **FraseKill Admin → Script settings**.

## Administration panel

The panel lets you change most common options visually: language, colours, FraseKill defaults, death detection, access, Tebex, rules and notifications.

Every option has a `?` that explains what it does in simple language.

If you choose **Configuration files**, the panel options are locked so it is clear that changes must be made in the files.

## Configuration files

### `config.lua`

General, non-private settings such as language, appearance, commands, defaults, animations and visual behaviour.

### `config_server.lua`

Server-only settings such as access, administration, Tebex, security and other internal options.

### `server/webhooks.lua`

Discord webhook URLs, if you want to use logs.

{% hint style="info" %}
If you are not used to configuring scripts, use the **Administration panel** for normal settings and edit files only when the documentation tells you to.
{% endhint %}
