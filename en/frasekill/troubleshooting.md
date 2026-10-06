# Troubleshooting

## `/frasekill` does not open

- Confirm the player has effective access.
- Check `Config.Access.Mode`.
- Run `/frasekillstatus` as an administrator.
- Check F8 and server console.

## Admin panel does not open

Verify the owner ACE and restart after changing it:

```cfg
add_ace identifier.license:YOUR_LICENSE zbrou.frasekill.admin allow
```

Delegated admins are managed from the panel; they do not need their own player-use ACE.

## Script settings are grey/locked

This is expected when **Configuration files** is selected. The owner must switch to **Administration panel** to edit supported settings in the UI.

## Medical detection is wrong

Run `/frasekillstatus`, check `Config.Death.Preferred` and verify the exact resource name. You can force `Config.Death.Adapter` or use the custom server-side death check.

## Database tables are missing

Start `oxmysql` first. With AutoCreate disabled, apply the appropriate files from `sql/`.

## Tebex does not grant access

Check `Config.Tebex.Enabled`, use `managed_tebex`, make sure the plan key is correct and ensure the command is executed by Tebex/console, not a player.

## UI colours look wrong

Use the separate detail/background/base pickers. Each menu colour has an individual reset icon, and the owner can use global **Restore defaults** to clear all Script settings overrides.
