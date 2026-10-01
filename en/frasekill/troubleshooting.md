# Troubleshooting

## `/frasekill` does not open

- Confirm the player has effective access.
- Run `/frasekillstatus` as an administrator.
- Check F8 and the server console for errors.

## Database tables are not created

- Make sure `oxmysql` starts before `zbrou_frasekill`.
- Verify database credentials.
- If automatic creation is disabled, run `sql/install.sql` manually.

## Admin panel does not open

Add the correct ACE to `server.cfg` and restart the resource:

```cfg
add_ace identifier.license:YOUR_LICENSE zbrou.frasekill.admin allow
```

## FraseKill appears behind another NUI

Increase `Config.NuiZIndex` only if another fullscreen resource renders above it.

## FraseKill does not hide on revive

- Review `Config.Display.Mode`.
- Check the adapter shown by `/frasekillstatus`.
- `FailsafeSeconds` is the safety limit for `death_state`.

## Tebex does not grant access

- Check `Config.Tebex.Enabled`.
- The delivery command must run from console/Tebex, not from a player.
- Make sure the plan name exactly matches the configured key.

## Need help?

Open **Support** to join the official Discord.
