# Configuration

FraseKill can be configured from the **visual Script settings panel** or directly from `config.lua` and `config_server.lua`.

## Visual configuration panel

{% embed url="https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=en" %}

[**Open the configuration panel full screen →**](https://raw.githack.com/zbrouscripts/docs/main/site/frasekill/index.html?lang=en)

The panel covers most common settings without editing code. Private options stay in the resource files.

## Configuration files

- `config.lua` — language, appearance, commands and default values.
- `config_server.lua` — access, administration, Tebex, security and server options.
- `server/webhooks.lua` — Discord webhooks.

## Permissions and administration

Add the main owner in `server.cfg`:

```cfg
add_ace identifier.license:YOUR_LICENSE zbrou.frasekill.admin allow
```

If you do not know your license, run `/frasekilladmin` and FraseKill will show the exact line.

Other administrators are created from the panel with separate permissions. Admin status does not automatically grant player access to FraseKill.
