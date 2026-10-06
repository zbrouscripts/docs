# Configuration

FraseKill can be configured in two ways: from the **visual Script settings panel**, which lets you change most options from `config.lua` and `config_server.lua` without editing code, or by editing those files directly.

Some private options, such as webhooks and other sensitive settings, always stay in the resource files.

## Visual configuration panel

This is the same type of panel you will find inside FraseKill Admin. You can try it here before changing anything on your server.

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=en" %}

[**Open the configuration panel full screen →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=en)

{% hint style="info" %}
The demo does not connect to FiveM, SQL or Tebex and never changes a server.
{% endhint %}

## Configure from files

### `config.lua`

General settings such as language, appearance, commands, defaults, animations and visual behaviour.

### `config_server.lua`

Server settings such as access, administration, Tebex, security and other internal options.

### `server/webhooks.lua`

Discord webhook URLs, if you want to use logs.

{% hint style="info" %}
If you are not used to configuring scripts, the easiest option is to use the **visual panel** for normal settings and edit files only when needed.
{% endhint %}
