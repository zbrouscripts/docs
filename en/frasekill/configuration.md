# Configuration

FraseKill can be configured in two ways:

- **From the administration panel**, which is the easiest option if you do not want to edit files.
- **From the configuration files**, if you prefer to keep everything in Lua.

Choose the mode from **FraseKill Admin → Script settings**.

## Administration panel

The panel lets you change most common options visually: language, colours, FraseKill defaults, death detection, access, Tebex, rules and notifications.

Every option has a `?` that explains what it does in simple language.

If you choose **Configuration files**, the panel options are locked so it is clear that changes must be made in the files.

## Try the panel before configuring it

Open an **interactive Script settings demo** using the same visual style as the real panel. You can try Classic/Liquid Glass, colours, switches, dropdowns, Configuration files lock mode and Restore defaults.

The demo follows the real panel structure: one scrollable screen, blocks in the same order, and the fixed action bar at the bottom.

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=en" %}

[**Open the full-screen demo →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=en)

{% hint style="info" %}
This is documentation-only: it does not connect to FiveM, SQL or Tebex and never changes a server.
{% endhint %}

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
