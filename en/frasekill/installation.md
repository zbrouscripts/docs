# Installation

## What you need

- A FiveM server.
- The `oxmysql` resource on your server.
- ESX, QBCore and Qbox are optional. FraseKill can also run without a framework.
- `zbrou_utils` is not required.

## Add FraseKill to your server

1. Put the folder in your resources and keep the name:

```text
zbrou_frasekill
```

2. In `server.cfg`, make sure `oxmysql` is listed before FraseKill:

```cfg
ensure oxmysql
ensure zbrou_frasekill
```

3. The required SQL is prepared automatically the first time FraseKill starts. An `sql/install.sql` file is also included if you prefer to prepare it manually.

4. Restart the resource or server.

## Give the owner access

FraseKill uses one ACE for the main owner:

```cfg
add_ace identifier.license:YOUR_LICENSE zbrou.frasekill.admin allow
```

If you run `/frasekilladmin` without permission, FraseKill shows the exact line you need to copy.

## Test FraseKill while setting up your server

`/frasekilltest` is disabled in the public version.

If you are setting up the server on your own and want to use it, open `config.lua`, find:

```lua
Config.Developer = {
    Enabled = false,
    Command = 'frasekilltest',
    RequireAdmin = true,
}
```

and change only:

```lua
Enabled = true
```

Keep `RequireAdmin = true` so only the owner/admin can run the test. Set `Enabled = false` again when you finish.
