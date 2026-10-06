# Permissions and administration

## Owner

FraseKill uses one ACE only:

```cfg
add_ace identifier.license:YOUR_LICENSE zbrou.frasekill.admin allow
```

This ACE gives the main owner full admin authority. It does **not** automatically give player-use access to FraseKill.

## Delegated administrators

The owner can create administrators inside the panel and grant individual permissions such as viewing profiles, granting/revoking access, editing/resetting phrases, deleting profiles, messaging players, editing rules, managing blocked words and configuring the script.

Delegated admin permissions are stored in SQL and remain separate from player access.

## Player access modes

`Config.Access.Mode` supports only:

- `managed` — access granted by FraseKill player/job/group grants.
- `managed_tebex` — managed access plus active Tebex entitlements.
- `custom` — your server-side `Config.Access.CustomCheck`.

There is no player-use ACE mode.

## Temporary access

Managed grants can be permanent or time-limited. Expiry is checked server-side. If another valid source still grants access, FraseKill does not incorrectly report that the player lost all access.
