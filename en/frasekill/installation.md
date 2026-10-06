# Installation

## Requirements

- FiveM server.
- `oxmysql` running before FraseKill.
- ESX, QBCore or Qbox are optional; standalone is supported.
- `zbrou_utils` is **not** required.

## Install

1. Put the folder in your resources directory and keep the resource name `zbrou_frasekill`.
2. Add:

```cfg
ensure oxmysql
ensure zbrou_frasekill
```

3. Leave `Config.Storage.AutoCreate = true` for automatic table creation/migrations, or run `sql/install.sql` manually if you manage SQL yourself.
4. Restart the server/resource and reconnect.

## First owner

The only ACE used by FraseKill is the owner/admin ACE:

```cfg
add_ace identifier.license:YOUR_LICENSE zbrou.frasekill.admin allow
```

You can also run `/frasekilladmin` without permission: FraseKill shows the exact line for your license. Restart after changing ACE permissions.

## First checks

- `/frasekill` opens the editor only if the player has access.
- `/frasekilladmin` opens the admin panel for the owner or delegated admins.
- `/frasekillstatus` shows diagnostics to administrators.
- `/frasekilltest` is disabled by default and should only be enabled on a test server.
