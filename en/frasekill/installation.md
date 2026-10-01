# Installation

## Quick start

1. Install and start `oxmysql`.
2. Add `zbrou_frasekill` to your server.
3. Review permissions and configuration before opening the server to players.
4. Add to `server.cfg`:

```cfg
ensure oxmysql
ensure zbrou_frasekill
```

5. Restart the resource or server.

FraseKill automatically creates and migrates its tables when `Config.Storage.AutoCreate = true`, which is the default. If you prefer a manual database setup, you can also run `sql/install.sql`.

## First administrator

Run:

```text
/frasekilladmin
```

If you do not have permission yet, the menu shows the exact ACE line to copy into `server.cfg`. You can also add it manually:

```cfg
add_ace identifier.license:YOUR_LICENSE zbrou.frasekill.admin allow
```

Restart the resource after changing ACE permissions.

## Check

- `/frasekill` opens the editor when the player has access.
- `/frasekilladmin` opens the administration panel.
- `/frasekillstatus` shows diagnostics to administrators.

`/frasekilltest` is a development-only tool and is disabled in the public release.
