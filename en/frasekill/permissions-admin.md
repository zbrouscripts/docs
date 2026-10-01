# Permissions and administration

## Open the panel

```text
/frasekilladmin
```

ACE is the recommended way to protect the admin panel:

```cfg
add_ace identifier.license:YOUR_LICENSE zbrou.frasekill.admin allow
```

If you open the panel without permission, FraseKill displays the ready-to-copy ACE line with your own identifier.

## Player access

The **Access** tab can grant access to online players by ID or by a supported identifier. Persistent permissions are stored with a stable identifier, not the temporary session ID.

Access can be permanent or last for minutes, hours, days, weeks, months or years.

## Jobs and groups

Available group systems depend on `Config.GroupAccess` in `config_server.lua`. Jobs, GuilleGangs V2, QB/Qbox gangs and custom resolvers can be enabled, including minimum grades.

## Phrases

The **Phrases** tab lets admins search users, open details, edit presets, reset/delete settings, grant/revoke manual access, save internal notes and send a message to an online player.

## Security

Important actions are validated again on the server. Never rely on NUI/client permissions as the only security layer.
